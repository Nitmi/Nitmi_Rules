# Maintenance Notes

## Shared shopping CDNs

- Do not add `DOMAIN-SUFFIX,alicdn.com` to `rule/Germany_Ecommerce.list`.
  This shared CDN also serves Taobao images such as `img.alicdn.com`.
  The shopping rule runs before China direct rules, so the broad suffix routed
  those images through the overseas shopping proxy and caused loading failures.
- Maintain the LIST source and regenerate its Domain YAML and MRS together.
  `auto-generate-rules.yml` already watches `Germany_Ecommerce.list`.
- Validate that Taobao image hosts no longer match this shopping ruleset while
  dedicated shopping domains such as `aliexpress.com` remain covered.
