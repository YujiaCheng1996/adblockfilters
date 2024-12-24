# AdBlock DNS Filters
适用于AdGuard的去广告合并规则，每8个小时更新一次。
个人收藏了不少广告过滤规则，但是每次往新设备添加的时候很是头疼，于是写了这个项目，定时自动获取各规则源更新，生成合并规则库。

## 说明
1. 定时从上游各规则源获取更新，合并去重。
2. 使用国内、国外各 3 组 DNS 服务，分别对上游各规则源拦截的域名进行解析，去除已无法解析的域名。（上游各规则源中存在大量已无法解析的域名，无需加入拦截规则）
3. 本项目仅对上游规则进行合并、去重、去除无效域名，不做任何修改。如发现误拦截情况，可临时添加放行规则（如 `@@||www.example.com^$important`），并向上游规则反馈。

## 订阅链接
1. AdGuard Home 等 DNS 拦截服务使用规则1
2. AdGuard 等浏览器插件使用规则1 + 规则2
3. 规则1’、规则2’为相应的 Lite 版，仅针对国内域名拦截

| 规则 | 原始链接 | 加速链接 |
|:-|:-|:-|
| 规则1：DNS 拦截 | [原始链接](https://raw.githubusercontent.com/YujiaCheng1996/adblockfilters/main/rules/adblockdns.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/adblockdns.txt) |
| 规则1'：DNS 拦截 Lite | [原始链接](https://raw.githubusercontent.com/YujiaCheng1996/adblockfilters/main/rules/adblockdnslite.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/adblockdnslite.txt) |
| 规则2：插件拦截 | [原始链接](https://raw.githubusercontent.com/YujiaCheng1996/adblockfilters/main/rules/adblockfilters.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/adblockfilters.txt) |
| 规则2'：插件拦截 Lite | [原始链接](https://raw.githubusercontent.com/YujiaCheng1996/adblockfilters/main/rules/adblockfilterslite.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/adblockfilterslite.txt) |

## 上游规则源
感谢各位广告过滤规则维护大佬们的辛苦付出。

| 规则 | 类型 | 原始链接 | 加速链接 | 更新日期 |
|:-|:-|:-|:-|:-|
| AdGuard Base filter | filter | [原始链接](https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_2_Base/filter.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AdGuard_Base_filter.txt) | 2024/12/25 |
| AdGuard Chinese filter | filter | [原始链接](https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_224_Chinese/filter.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AdGuard_Chinese_filter.txt) | 2024/12/25 |
| AdGuard Mobile Ads filter | filter | [原始链接](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/MobileFilter/sections/adservers.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AdGuard_Mobile_Ads_filter.txt) | 2024/12/07 |
| AdGuard DNS filter | filter | [原始链接](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AdGuard_DNS_filter.txt) | 2024/12/25 |
| uBlock filter | filter | [原始链接](https://github.com/uBlockOrigin/uAssets/blob/master/filters/filters.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/uBlock_filter.txt) | 2024/09/25 |
| EasyList | filter | [原始链接](https://easylist-downloads.adblockplus.org/easylist.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/EasyList.txt) | 2024/12/25 |
| EasyList China | filter | [原始链接](https://easylist-downloads.adblockplus.org/easylistchina.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/EasyList_China.txt) | 2024/12/25 |
| EasyPrivacy | filter | [原始链接](https://easylist-downloads.adblockplus.org/easyprivacy.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/EasyPrivacy.txt) | 2024/12/25 |
| CJX's Annoyance List | filter | [原始链接](https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjx-annoyance.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/CJX's_Annoyance_List.txt) | 2024/12/22 |
| xinggsf rule | filter | [原始链接](https://raw.githubusercontent.com/xinggsf/Adblock-Plus-Rule/master/rule.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/xinggsf_rule.txt) | 2024/11/19 |
| xinggsf mv | filter | [原始链接](https://raw.githubusercontent.com/xinggsf/Adblock-Plus-Rule/master/mv.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/xinggsf_mv.txt) | 2024/12/17 |
| SmartTV Blocklist | filter | [原始链接](https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV-AGH.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/SmartTV_Blocklist.txt) | 2024/11/19 |
| halflife | filter | [原始链接](https://raw.githubusercontent.com/o0HalfLife0o/list/master/ad.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/halflife.txt) | 2024/12/25 |
| NoAppDownload | filter | [原始链接](https://raw.githubusercontent.com/Noyllopa/NoAppDownload/master/NoAppDownload.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/NoAppDownload.txt) | 2024/12/08 |
| QuarkList | filter | [原始链接](https://raw.githubusercontent.com/francis-zhao/quarklist/master/dist/quarklist.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/QuarkList.txt) | 2024/11/19 |
| DD-AD | filter | [原始链接](https://raw.githubusercontent.com/afwfv/DD-AD/main/rule/DD-AD.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/DD-AD.txt) | 2024/12/08 |
| banad | filter | [原始链接](https://raw.githubusercontent.com/damengzhu/banad/main/jiekouAD.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/banad.txt) | 2024/12/21 |
| Ad Filter J | filter | [原始链接](https://raw.githubusercontent.com/jk278/Ad-J/main/Ad-J.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/Ad_Filter_J.txt) | 2024/11/19 |
| Fuck Fuckadblock | filter | [原始链接](https://raw.githubusercontent.com/bogachenko/fuckfuckadblock/master/fuckfuckadblock.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/Fuck_Fuckadblock.txt) | 2024/11/19 |
| GOODBYEADS | dns | [原始链接](https://raw.githubusercontent.com/8680/GOODBYEADS/master/data/rules/adblock.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/GOODBYEADS.txt) | 2024/12/25 |
| 1Hosts (Lite) | dns | [原始链接](https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/1Hosts_(Lite).txt) | 2024/12/16 |
| AdRules DNS List | dns | [原始链接](https://raw.githubusercontent.com/Cats-Team/AdRules/main/dns.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AdRules_DNS_List.txt) | 2024/12/25 |
| NEO DEV HOST | dns | [原始链接](https://raw.githubusercontent.com/neodevpro/neodevhost/master/adblocker) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/NEO_DEV_HOST.txt) | 2024/12/24 |
| OISD Big | dns | [原始链接](https://raw.githubusercontent.com/sjhgvr/oisd/main/abp_big.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/OISD_Big.txt) | 2024/12/25 |
| AWAvenue Ads Rule | dns | [原始链接](https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/AWAvenue_Ads_Rule.txt) | 2024/12/22 |
| d3ward | dns | [原始链接](https://raw.githubusercontent.com/d3ward/toolz/master/src/d3host.adblock) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/d3ward.txt) | 2024/11/19 |
| BlueSkyXN skyrules | dns | [原始链接](https://raw.githubusercontent.com/BlueSkyXN/AdGuardHomeRules/master/skyrules.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/BlueSkyXN_skyrules.txt) | 2024/11/19 |
| mitv-blacklist | dns | [原始链接](https://raw.githubusercontent.com/Chriser001/mitv-blacklist/main/mitv-blacklist.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/mitv-blacklist.txt) | 2024/11/19 |
| 1024 hosts | host | [原始链接](https://raw.githubusercontent.com/Goooler/1024_hosts/master/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/1024_hosts.txt) | 2024/11/19 |
| ad-wars hosts | host | [原始链接](https://raw.githubusercontent.com/jdlingyu/ad-wars/master/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/ad-wars_hosts.txt) | 2024/11/19 |
| StevenBlack hosts | host | [原始链接](https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/gambling/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/StevenBlack_hosts.txt) | 2024/12/24 |
| QuarkList hosts | host | [原始链接](https://raw.githubusercontent.com/francis-zhao/quarklist/master/dist/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/QuarkList_hosts.txt) | 2024/11/19 |
| ilpl | host | [原始链接](https://raw.githubusercontent.com/ilpl/ad-hosts/master/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/ilpl.txt) | 2024/11/19 |
| xiaobeita | host | [原始链接](https://raw.githubusercontent.com/rentianyu/Ad-set-hosts/master/xiaobeita/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/xiaobeita.txt) | 2024/11/19 |
| WindowsSpyBlocker | host | [原始链接](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/WindowsSpyBlocker.txt) | 2024/11/19 |
| eth-phishing-detect | host | [原始链接](https://raw.githubusercontent.com/MetaMask/eth-phishing-detect/master/src/hosts.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/eth-phishing-detect.txt) | 2024/11/19 |
| Badd-Boyz-Hosts | host | [原始链接](https://raw.githubusercontent.com/mitchellkrogza/Badd-Boyz-Hosts/master/hosts) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/Badd-Boyz-Hosts.txt) | 2024/11/19 |
| URLhaus | host | [原始链接](https://urlhaus.abuse.ch/downloads/hostfile) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/URLhaus.txt) | 2024/12/25 |
| DigitalSide Threat-Intel | host | [原始链接](https://osint.digitalside.it/Threat-Intel/lists/latestdomains.piHole.txt) | [加速链接](https://quantil.jsdelivr.net/gh/YujiaCheng1996/adblockfilters@main/rules/DigitalSide_Threat-Intel.txt) | 2024/11/19 |

