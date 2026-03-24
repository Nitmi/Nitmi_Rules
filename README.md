# Nitmi Rules

## 项目包含

### 1. Loon 配置

- [一键导入 Nitmi Loon 配置](https://www.nsloon.com/openloon/import?sub=https%3A%2F%2Fgh.123778.xyz%2FNitmi_Rules%2Fmain%2Floon%2FLoon_Nitmi_Full.conf)
- 配置文件：`loon/Loon_Nitmi_Full.conf`
- 配置 URL：[https://gh.123778.xyz/Nitmi_Rules/main/loon/Loon_Nitmi_Full.conf](https://gh.123778.xyz/Nitmi_Rules/main/loon/Loon_Nitmi_Full.conf)

<p align="center">
  <img src="docs/screenshot.png" alt="Nitmi Rules Screenshot" width="420">
</p>

### 2. 传统订阅转换配置

- 适配 [SubConverter-Extended](https://github.com/Aethersailor/SubConverter-Extended) 订阅转换后端增强版，同时兼容常规版 [SubConverter](https://github.com/tindy2013/subconverter)
- 配置文件：`convert/Custom_Clash_Full.ini`
- 配置 URL：[https://gh.123778.xyz/Nitmi_Rules/main/convert/Custom_Clash_Full.ini](https://gh.123778.xyz/Nitmi_Rules/main/convert/Custom_Clash_Full.ini)

## Loon 小白使用教程

1. [一键导入 Nitmi Loon 配置](https://www.nsloon.com/openloon/import?sub=https%3A%2F%2Fgh.123778.xyz%2FNitmi_Rules%2Fmain%2Floon%2FLoon_Nitmi_Full.conf)
   注意：**一定要关闭“全覆盖更新”**。
2. 按照可莉的 Loon 设置图完成 Loon 必要设置。  
   设置参考图：[ConfigDiagram.png](https://raw.githubusercontent.com/luestr/ProxyResource/main/Tool/Loon/Lcf/zh-CN/Resource/ConfigDiagram.png)
3. 购买机场服务并导入机场节点，常见情况如下：
   - 机场有一键导入 Loon 的，直接点击即可。
   - 机场有“复制订阅地址”的，使用 Loon 的“节点 -> 添加订阅 -> URL”，粘贴订阅地址导入。
   - 机场支持 Shadowrocket 的，Shadowrocket 用的链接一般也可以在 Loon 中使用。
   - 以上都不行的，使用 sub-store 转换。
   - 如果还不行，那通常就是你的机场节点协议 Loon 不支持。
4. 按需安装插件。  
   插件不宜过多，安装常用的就好。  
   插件市场推荐：[https://hub.kelee.one](https://hub.kelee.one)
5. 完成以上步骤后，再根据自己的使用习惯微调分组、插件和策略。  
   小白不建议一开始就装太多插件或频繁改配置。

## 传统订阅转换教程

Loon 用户更推荐直接使用上面的 Loon 配置导入方式，而不是传统订阅转换。

为什么要订阅转换：

- 使用的客户端不支持机场原始订阅
- 机场自带的分流规则不好用
- 需要把多个机场服务融合到一个链接中
- 相比手搓配置文件，这种方式对小白更友好

使用步骤：

1. 复制机场订阅链接。
2. 打开 [订阅转换增强版的前端网页](https://sub-converter.123778.xyz)。
3. 按提示填写各项内容。
4. 生成订阅转换链接，导入到 Clash 系以及其他客户端。

## 项目参考

- [Aethersailor/Custom_OpenClash_Rules](https://github.com/Aethersailor/Custom_OpenClash_Rules/tree/main)
- [Sleepstars/Surge-Geosite-Enhance](https://github.com/Sleepstars/Surge-Geosite-Enhance)
- [luestr/ProxyResource](https://github.com/luestr/ProxyResource)
- [fmz200/wool_scripts](https://github.com/fmz200/wool_scripts)
- [Tartarus2014/Loon-Script](https://github.com/Tartarus2014/Loon-Script)
- [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)
- [ACL4SSR/ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master)
- [Loon 文档](https://nsloon.app/docs/intro)
- [LoonExampleConfig](https://github.com/Loon0x00/LoonExampleConfig)
