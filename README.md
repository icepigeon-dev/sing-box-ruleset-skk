# 🚀 Sing-box 规则集 (预编译二进制版本)

> **自动同步编译** | **开箱即用** | **高性能二进制格式**

本仓库自动从 [SukkaLab/ruleset.skk.moe](https://github.com/SukkaLab/ruleset.skk.moe) 同步 sing-box 规则集源文件，并编译为高性能的二进制格式 (`.srs`)，方便直接在 sing-box 配置中使用。

## 📥 快速使用

在你的 sing-box 配置文件中直接引用编译后的规则集：

```json
{
  "rule_set": [
    {
      "tag": "geosite-category-ads-all",
      "type": "remote",
      "format": "binary",
      "url": "https://icepigeon-dev.github.io/sing-box-ruleset-skk/sing-box/geosite-category-ads-all.srs",
      "download_detour": "direct"
    }
  ],
  "rules": [
    {
      "rule_set": "geosite-category-ads-all",
      "outbound": "block"
    }
  ]
}
```

## 🎯 优势特点
- ✅ **预编译**: 二进制格式加载速度快
- ✅ **自动更新**: 无需手动维护，始终保持最新
- ✅ **轻量同步**: 仅同步必要文件，节省带宽
- ✅ **稳定可靠**: GitHub Actions 自动化流程
- ✅ **开源透明**: 完整的构建过程可追溯

## 🔗 相关链接

- [原始规则集仓库](https://github.com/SukkaLab/ruleset.skk.moe)
- [Sing-box 官方文档](https://sing-box.sagernet.org/)
- [规则集配置说明](https://sing-box.sagernet.org/configuration/rule-set/)

## 📄 许可证

本仓库遵循源仓库的许可证条款。编译脚本采用 MIT 许可证。

