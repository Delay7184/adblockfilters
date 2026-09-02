# AdBlock DNS Filters
去广告合并规则，每8个小时更新一次。  
个人收藏了不少广告过滤规则，但是每次往新设备添加的时候很是头疼，于是写了这个项目，定时自动获取各规则源更新，生成合并规则库。

## 说明
1. 定时从上游各规则源获取更新，合并去重。
2. 使用国内、国外各 3 组 DNS 服务，分别对上游各规则源拦截的域名进行解析，去除已无法解析的域名。
3. 本项目仅对上游规则进行合并、去重、去除无效域名，不做任何修改。如发现误拦截情况，可临时添加放行规则（如 `@@||www.example.com^$important`）。

## 订阅链接
1. 规则x'为规则x的 Lite 版，仅针对国内域名拦截，体积较小（如添加完整规则报错数量限制，请尝试 Lite 规则）
2. 已对 jsdelivr(加速链接1) 缓存进行主动刷新，但仍存在一定刷新延时

| 规则 | 原始链接 | 加速链接1 | 加速链接2 | 加速链接3 | 适配说明 |
|:-|:-|:-|:-|:-|:-|
| 规则1 | [原始链接](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | DNS-Blocklists PRO |
| 规则1' | [原始链接](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | DNS-Blocklists PRO Lite |
| 规则2 | [原始链接](https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/TG-Twilight/AWAvenue-Ads-Rule@main/AWAvenue-Ads-Rule.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | AWAvenue Ads Rule |
| 规则2' | [原始链接](https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/TG-Twilight/AWAvenue-Ads-Rule@main/AWAvenue-Ads-Rule.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | AWAvenue Ads Rule Lite |

## 上游规则源
感谢以下规则维护者的辛苦付出。

| 规则 | 类型 | 原始链接 | 加速链接1 | 加速链接2 | 加速链接3 | 更新日期 |
|:-|:-|:-|:-|:-|:-|:-|
| DNS-Blocklists PRO | dns | [原始链接](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt) | 2024/01/01 |
| AWAvenue Ads Rule | dns | [原始链接](https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接1](https://gcore.jsdelivr.net/gh/TG-Twilight/AWAvenue-Ads-Rule@main/AWAvenue-Ads-Rule.txt) | [加速链接2](https://github.boki.moe/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接3](https://ghfast.top/https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | 2024/01/01 |
