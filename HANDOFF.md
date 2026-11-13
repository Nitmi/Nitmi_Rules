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

## Actions unavailable

- GitHub may block jobs before startup with an account billing error. This does
  not mean generated files already committed and pushed are missing.
- Generate YAML and MRS locally when Actions is unavailable. The installed
  `C:\Program Files\Clash Verge\verge-mihomo.exe` supports
  `convert-ruleset domain yaml <source.yaml> <target.mrs>`; decode with
  `convert-ruleset domain mrs <source.mrs> <target.txt>` to verify the payload.
- Check the published LIST, YAML and MRS hashes on both GitHub Raw and the
  configured subscription CDN before attempting a manual cache purge. The
  AliCDN fix was verified on both endpoints without a successful purge job.
