# fenliu

Clash Mini / subconverter 用的分流外部配置。

## 文件

- `dollei-final.ini`：基于 `final.yaml` 分流规则整理的 mini 配置。

## 分流策略

当前配置保留了 `final.yaml` 的主要分流组：

- `AI`
- `Meta AI`
- `Google`
- `Perplexity`
- `Stream Media`
- `GitHub`
- `Reddit`
- `Nvidia`
- `Apple`
- `Microsoft`
- `Games`
- `Crypto`
- `Test`
- `Block`
- `国外`
- `国内`
- `其他`

节点策略组包含：

- `所有-手动`
- `所有-自动`
- `家宽`
- `香港-自动` / `香港-故转`
- `台湾-故转`
- `日本-故转`
- `新加坡-故转`
- `美国-故转`
- `其他-故转`

## 使用

raw 地址：

```text
https://raw.githubusercontent.com/dollei-jay/fenliu/main/dollei-final.ini
```

在支持 subconverter 外部配置的订阅转换服务中，将上面的 raw 地址填入外部配置地址即可。

配置中已启用：

```ini
enable_rule_generator=true
overwrite_original_rules=true
```

## 说明

`final.yaml` 中使用的部分 `.mrs` 规则源在 mini / subconverter 场景下兼容性不如 `.list` 稳定，因此本配置将这些规则源替换成了可直接处理的 `clash-classic:`、`clash-domain:`、`clash-ipcidr:` 格式。
