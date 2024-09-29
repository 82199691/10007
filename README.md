# 致谢

感谢10007整理众多广告规则

<a href="https://github.com/lingeringsound">

  <p align="center">
    <img src="https://avatars.githubusercontent.com/u/114198798?v=4" width="100" height="100" alt="lingeringsound">
    <br>
    <strong>lingeringsound</strong>
  </p>

</a>

## 使用说明

本规则自动转换10007广告规则中保留广告奖励规则

引用链接

> https://raw.githubusercontent.com/82199691/10007/refs/heads/master/singbox_rules.json

### sing-box引用示例

  DNS部分：

```json
    "rules": [
      {
        "rule_set": "10007_rule",
        "server": "block"
      }],


```

route部分：

```json
"route": {
    "rule_set": [
      {
        "tag": "geoip-cn",
        "type": "remote",
        "format": "binary",
        "url": "https://raw.githubusercontent.com/82199691/10007/refs/heads/master/singbox_rules.json",
        "download_detour": "direct"
      }
    ],
    
```



```json
"rules": [
  {
    "rule_set": [
      "10007_rule"
    ],
    "outbound": "block"
   }
```



