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
      "url": "[https://raw.githubusercontent.com/$](https://raw.githubusercontent.com/$){GITHUB_REPOSITORY}/main/sing-box/geosite-category-ads-all.srs",
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

## 📋 可用规则集

| 规则集名称 | 描述 | JSON源文件 | SRS编译文件 | 文件大小 |
|------------|------|------------|-------------|----------|
| `apple_cdn` | 规则集 | [`sing-box/domainset/apple_cdn.json`](sing-box/domainset/apple_cdn.json) | [`sing-box/domainset/apple_cdn.srs`](sing-box/domainset/apple_cdn.srs) | 1.5K |
| `cdn` | 规则集 | [`sing-box/domainset/cdn.json`](sing-box/domainset/cdn.json) | [`sing-box/domainset/cdn.srs`](sing-box/domainset/cdn.srs) | 29K |
| `download` | 规则集 | [`sing-box/domainset/download.json`](sing-box/domainset/download.json) | [`sing-box/domainset/download.srs`](sing-box/domainset/download.srs) | 11K |
| `game-download` | 规则集 | [`sing-box/domainset/game-download.json`](sing-box/domainset/game-download.json) | [`sing-box/domainset/game-download.srs`](sing-box/domainset/game-download.srs) | 745 |
| `icloud_private_relay` | 规则集 | [`sing-box/domainset/icloud_private_relay.json`](sing-box/domainset/icloud_private_relay.json) | [`sing-box/domainset/icloud_private_relay.srs`](sing-box/domainset/icloud_private_relay.srs) | 163 |
| `reject` | 规则集 | [`sing-box/domainset/reject.json`](sing-box/domainset/reject.json) | [`sing-box/domainset/reject.srs`](sing-box/domainset/reject.srs) | 726K |
| `reject_extra` | 规则集 | [`sing-box/domainset/reject_extra.json`](sing-box/domainset/reject_extra.json) | [`sing-box/domainset/reject_extra.srs`](sing-box/domainset/reject_extra.srs) | 392K |
| `reject_phishing` | 规则集 | [`sing-box/domainset/reject_phishing.json`](sing-box/domainset/reject_phishing.json) | [`sing-box/domainset/reject_phishing.srs`](sing-box/domainset/reject_phishing.srs) | 1.8M |
| `speedtest` | 规则集 | [`sing-box/domainset/speedtest.json`](sing-box/domainset/speedtest.json) | [`sing-box/domainset/speedtest.srs`](sing-box/domainset/speedtest.srs) | 14K |
| `apple_services` | 规则集 | [`sing-box/ip/apple_services.json`](sing-box/ip/apple_services.json) | [`sing-box/ip/apple_services.srs`](sing-box/ip/apple_services.srs) | 176 |
| `cdn` | 规则集 | [`sing-box/ip/cdn.json`](sing-box/ip/cdn.json) | [`sing-box/ip/cdn.srs`](sing-box/ip/cdn.srs) | 108 |
| `china_ip` | 规则集 | [`sing-box/ip/china_ip.json`](sing-box/ip/china_ip.json) | [`sing-box/ip/china_ip.srs`](sing-box/ip/china_ip.srs) | 16K |
| `china_ip_ipv6` | 规则集 | [`sing-box/ip/china_ip_ipv6.json`](sing-box/ip/china_ip_ipv6.json) | [`sing-box/ip/china_ip_ipv6.srs`](sing-box/ip/china_ip_ipv6.srs) | 6.3K |
| `domestic` | 规则集 | [`sing-box/ip/domestic.json`](sing-box/ip/domestic.json) | [`sing-box/ip/domestic.srs`](sing-box/ip/domestic.srs) | 107 |
| `download` | 规则集 | [`sing-box/ip/download.json`](sing-box/ip/download.json) | [`sing-box/ip/download.srs`](sing-box/ip/download.srs) | 180 |
| `lan` | 规则集 | [`sing-box/ip/lan.json`](sing-box/ip/lan.json) | [`sing-box/ip/lan.srs`](sing-box/ip/lan.srs) | 175 |
| `neteasemusic` | 规则集 | [`sing-box/ip/neteasemusic.json`](sing-box/ip/neteasemusic.json) | [`sing-box/ip/neteasemusic.srs`](sing-box/ip/neteasemusic.srs) | 175 |
| `reject` | 规则集 | [`sing-box/ip/reject.json`](sing-box/ip/reject.json) | [`sing-box/ip/reject.srs`](sing-box/ip/reject.srs) | 604 |
| `stream` | 规则集 | [`sing-box/ip/stream.json`](sing-box/ip/stream.json) | [`sing-box/ip/stream.srs`](sing-box/ip/stream.srs) | 276 |
| `stream_biliintl` | 规则集 | [`sing-box/ip/stream_biliintl.json`](sing-box/ip/stream_biliintl.json) | [`sing-box/ip/stream_biliintl.srs`](sing-box/ip/stream_biliintl.srs) | 80 |
| `stream_eu` | 规则集 | [`sing-box/ip/stream_eu.json`](sing-box/ip/stream_eu.json) | [`sing-box/ip/stream_eu.srs`](sing-box/ip/stream_eu.srs) | 83 |
| `stream_hk` | 规则集 | [`sing-box/ip/stream_hk.json`](sing-box/ip/stream_hk.json) | [`sing-box/ip/stream_hk.srs`](sing-box/ip/stream_hk.srs) | 83 |
| `stream_jp` | 规则集 | [`sing-box/ip/stream_jp.json`](sing-box/ip/stream_jp.json) | [`sing-box/ip/stream_jp.srs`](sing-box/ip/stream_jp.srs) | 83 |
| `stream_kr` | 规则集 | [`sing-box/ip/stream_kr.json`](sing-box/ip/stream_kr.json) | [`sing-box/ip/stream_kr.srs`](sing-box/ip/stream_kr.srs) | 83 |
| `stream_tw` | 规则集 | [`sing-box/ip/stream_tw.json`](sing-box/ip/stream_tw.json) | [`sing-box/ip/stream_tw.srs`](sing-box/ip/stream_tw.srs) | 83 |
| `stream_us` | 规则集 | [`sing-box/ip/stream_us.json`](sing-box/ip/stream_us.json) | [`sing-box/ip/stream_us.srs`](sing-box/ip/stream_us.srs) | 83 |
| `telegram` | 规则集 | [`sing-box/ip/telegram.json`](sing-box/ip/telegram.json) | [`sing-box/ip/telegram.srs`](sing-box/ip/telegram.srs) | 190 |
| `telegram_asn` | 规则集 | [`sing-box/ip/telegram_asn.json`](sing-box/ip/telegram_asn.json) | [`sing-box/ip/telegram_asn.srs`](sing-box/ip/telegram_asn.srs) | 83 |
| `ai` | 规则集 | [`sing-box/non_ip/ai.json`](sing-box/non_ip/ai.json) | [`sing-box/non_ip/ai.srs`](sing-box/non_ip/ai.srs) | 460 |
| `apple_cdn` | 规则集 | [`sing-box/non_ip/apple_cdn.json`](sing-box/non_ip/apple_cdn.json) | [`sing-box/non_ip/apple_cdn.srs`](sing-box/non_ip/apple_cdn.srs) | 1.5K |
| `apple_cn` | 规则集 | [`sing-box/non_ip/apple_cn.json`](sing-box/non_ip/apple_cn.json) | [`sing-box/non_ip/apple_cn.srs`](sing-box/non_ip/apple_cn.srs) | 180 |
| `apple_services` | 规则集 | [`sing-box/non_ip/apple_services.json`](sing-box/non_ip/apple_services.json) | [`sing-box/non_ip/apple_services.srs`](sing-box/non_ip/apple_services.srs) | 352 |
| `cdn` | 规则集 | [`sing-box/non_ip/cdn.json`](sing-box/non_ip/cdn.json) | [`sing-box/non_ip/cdn.srs`](sing-box/non_ip/cdn.srs) | 894 |
| `cloudmounter` | 规则集 | [`sing-box/non_ip/cloudmounter.json`](sing-box/non_ip/cloudmounter.json) | [`sing-box/non_ip/cloudmounter.srs`](sing-box/non_ip/cloudmounter.srs) | 83 |
| `direct` | 规则集 | [`sing-box/non_ip/direct.json`](sing-box/non_ip/direct.json) | [`sing-box/non_ip/direct.srs`](sing-box/non_ip/direct.srs) | 1.7K |
| `domestic` | 规则集 | [`sing-box/non_ip/domestic.json`](sing-box/non_ip/domestic.json) | [`sing-box/non_ip/domestic.srs`](sing-box/non_ip/domestic.srs) | 4.6K |
| `download` | 规则集 | [`sing-box/non_ip/download.json`](sing-box/non_ip/download.json) | [`sing-box/non_ip/download.srs`](sing-box/non_ip/download.srs) | 178 |
| `gitlab` | 规则集 | [`sing-box/non_ip/gitlab.json`](sing-box/non_ip/gitlab.json) | [`sing-box/non_ip/gitlab.srs`](sing-box/non_ip/gitlab.srs) | 101 |
| `global` | 规则集 | [`sing-box/non_ip/global.json`](sing-box/non_ip/global.json) | [`sing-box/non_ip/global.srs`](sing-box/non_ip/global.srs) | 6.3K |
| `lan` | 规则集 | [`sing-box/non_ip/lan.json`](sing-box/non_ip/lan.json) | [`sing-box/non_ip/lan.srs`](sing-box/non_ip/lan.srs) | 463 |
| `microsoft` | 规则集 | [`sing-box/non_ip/microsoft.json`](sing-box/non_ip/microsoft.json) | [`sing-box/non_ip/microsoft.srs`](sing-box/non_ip/microsoft.srs) | 738 |
| `microsoft_cdn` | 规则集 | [`sing-box/non_ip/microsoft_cdn.json`](sing-box/non_ip/microsoft_cdn.json) | [`sing-box/non_ip/microsoft_cdn.srs`](sing-box/non_ip/microsoft_cdn.srs) | 331 |
| `my_direct` | 规则集 | [`sing-box/non_ip/my_direct.json`](sing-box/non_ip/my_direct.json) | [`sing-box/non_ip/my_direct.srs`](sing-box/non_ip/my_direct.srs) | 208 |
| `my_git` | 规则集 | [`sing-box/non_ip/my_git.json`](sing-box/non_ip/my_git.json) | [`sing-box/non_ip/my_git.srs`](sing-box/non_ip/my_git.srs) | 155 |
| `my_plus` | 规则集 | [`sing-box/non_ip/my_plus.json`](sing-box/non_ip/my_plus.json) | [`sing-box/non_ip/my_plus.srs`](sing-box/non_ip/my_plus.srs) | 241 |
| `my_proxy` | 规则集 | [`sing-box/non_ip/my_proxy.json`](sing-box/non_ip/my_proxy.json) | [`sing-box/non_ip/my_proxy.srs`](sing-box/non_ip/my_proxy.srs) | 228 |
| `my_reject` | 规则集 | [`sing-box/non_ip/my_reject.json`](sing-box/non_ip/my_reject.json) | [`sing-box/non_ip/my_reject.srs`](sing-box/non_ip/my_reject.srs) | 516 |
| `my_us` | 规则集 | [`sing-box/non_ip/my_us.json`](sing-box/non_ip/my_us.json) | [`sing-box/non_ip/my_us.srs`](sing-box/non_ip/my_us.srs) | 193 |
| `neteasemusic` | 规则集 | [`sing-box/non_ip/neteasemusic.json`](sing-box/non_ip/neteasemusic.json) | [`sing-box/non_ip/neteasemusic.srs`](sing-box/non_ip/neteasemusic.srs) | 121 |
| `reject-drop` | 规则集 | [`sing-box/non_ip/reject-drop.json`](sing-box/non_ip/reject-drop.json) | [`sing-box/non_ip/reject-drop.srs`](sing-box/non_ip/reject-drop.srs) | 158 |
| `reject-no-drop` | 规则集 | [`sing-box/non_ip/reject-no-drop.json`](sing-box/non_ip/reject-no-drop.json) | [`sing-box/non_ip/reject-no-drop.srs`](sing-box/non_ip/reject-no-drop.srs) | 136 |
| `reject-url-regex` | 规则集 | [`sing-box/non_ip/reject-url-regex.json`](sing-box/non_ip/reject-url-regex.json) | [`sing-box/non_ip/reject-url-regex.srs`](sing-box/non_ip/reject-url-regex.srs) | 83 |
| `reject` | 规则集 | [`sing-box/non_ip/reject.json`](sing-box/non_ip/reject.json) | [`sing-box/non_ip/reject.srs`](sing-box/non_ip/reject.srs) | 2.7K |
| `sogouinput` | 规则集 | [`sing-box/non_ip/sogouinput.json`](sing-box/non_ip/sogouinput.json) | [`sing-box/non_ip/sogouinput.srs`](sing-box/non_ip/sogouinput.srs) | 211 |
| `stream` | 规则集 | [`sing-box/non_ip/stream.json`](sing-box/non_ip/stream.json) | [`sing-box/non_ip/stream.srs`](sing-box/non_ip/stream.srs) | 2.6K |
| `stream_biliintl` | 规则集 | [`sing-box/non_ip/stream_biliintl.json`](sing-box/non_ip/stream_biliintl.json) | [`sing-box/non_ip/stream_biliintl.srs`](sing-box/non_ip/stream_biliintl.srs) | 188 |
| `stream_eu` | 规则集 | [`sing-box/non_ip/stream_eu.json`](sing-box/non_ip/stream_eu.json) | [`sing-box/non_ip/stream_eu.srs`](sing-box/non_ip/stream_eu.srs) | 174 |
| `stream_hk` | 规则集 | [`sing-box/non_ip/stream_hk.json`](sing-box/non_ip/stream_hk.json) | [`sing-box/non_ip/stream_hk.srs`](sing-box/non_ip/stream_hk.srs) | 491 |
| `stream_jp` | 规则集 | [`sing-box/non_ip/stream_jp.json`](sing-box/non_ip/stream_jp.json) | [`sing-box/non_ip/stream_jp.srs`](sing-box/non_ip/stream_jp.srs) | 347 |
| `stream_kr` | 规则集 | [`sing-box/non_ip/stream_kr.json`](sing-box/non_ip/stream_kr.json) | [`sing-box/non_ip/stream_kr.srs`](sing-box/non_ip/stream_kr.srs) | 124 |
| `stream_tw` | 规则集 | [`sing-box/non_ip/stream_tw.json`](sing-box/non_ip/stream_tw.json) | [`sing-box/non_ip/stream_tw.srs`](sing-box/non_ip/stream_tw.srs) | 434 |
| `stream_us` | 规则集 | [`sing-box/non_ip/stream_us.json`](sing-box/non_ip/stream_us.json) | [`sing-box/non_ip/stream_us.srs`](sing-box/non_ip/stream_us.srs) | 486 |
| `telegram` | 规则集 | [`sing-box/non_ip/telegram.json`](sing-box/non_ip/telegram.json) | [`sing-box/non_ip/telegram.srs`](sing-box/non_ip/telegram.srs) | 226 |

## 🔄 自动更新

- **同步频率**: 每天凌晨 2:00 UTC 自动检查更新
- **更新策略**: 仅同步 `sing-box` 目录，高效快速
- **编译**: 自动编译所有 JSON 规则集为二进制格式

## 📊 当前状态

- **最后更新**: 2025-06-02 01:25:55 UTC
- **源仓库提交**: [`be8d232`](https://github.com/SukkaLab/ruleset.skk.moe/commit/be8d23240134a5e99a8f26039f7c372d8301b1df)
- **规则集数量**: 63 个
- **总大小**: 15M

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

---

⭐ 如果这个仓库对你有帮助，请给个 Star 支持一下！
