# 规则配置

~~~yaml
[custom]
;不要随意改变关键字，否则会导致出错
;acl4SSR规则

;去广告：支持
;自动测速：支持
;微软分流：支持
;苹果分流：支持
;增强中国IP段：支持
;增强国外GFW：支持

; clash-rules项目提供的规则集
; 分流规则命名,规则同名最终会共同叠加生效
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list
ruleset=🍃 应用净化,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list
ruleset=📢 谷歌FCM,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/GoogleFCM.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/GoogleCN.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/SteamCN.list
ruleset=Ⓜ️ 微软Bing,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Bing.list
ruleset=Ⓜ️ 微软云盘,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/OneDrive.list
ruleset=Ⓜ️ 微软服务,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Microsoft.list
ruleset=🍎 苹果服务,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Apple.list
ruleset=📲 电报消息,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Telegram.list
ruleset=💬 OpenAi,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/OpenAi.list
ruleset=🎶 网易音乐,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/NetEaseMusic.list
ruleset=🎮 游戏平台,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Epic.list
ruleset=🎮 游戏平台,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Origin.list
ruleset=🎮 游戏平台,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Sony.list
ruleset=🎮 游戏平台,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Steam.list
ruleset=🎮 游戏平台,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Nintendo.list
ruleset=📹 油管视频,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/YouTube.list
ruleset=🎥 奈飞视频,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Netflix.list
ruleset=📺 巴哈姆特,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Bahamut.list
ruleset=📺 哔哩哔哩,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/BilibiliHMT.list
ruleset=📺 哔哩哔哩,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Bilibili.list
ruleset=🧩 国内媒体,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaMedia.list
ruleset=🌍 国外媒体,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ProxyMedia.list
ruleset=🚀 节点选择,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ProxyGFWlist.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Download.list
ruleset=🎯 全球直连,[]GEOIP,LAN
ruleset=🎯 全球直连,[]GEOIP,CN
ruleset=🐟 漏网之鱼,[]FINAL

;设置分组标志位：代理组名称`select或url-test    `.*: 表示加入你订阅中所有节点
;符合ruleset规则的节点：[]+ruleset的规则
custom_proxy_group=🚀 节点选择`select`[]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=♻️ 自动选择`url-test`.*`http://www.gstatic.com/generate_204`300,,50
custom_proxy_group=📲 电报消息`select`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=📹 油管视频`select`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=📺 哔哩哔哩`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=🌍 国外媒体`select`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=🧩 国内媒体`select`[]🎯 全球直连`.*
custom_proxy_group=📢 谷歌FCM`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=Ⓜ️ 微软Bing`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=Ⓜ️ 微软云盘`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=Ⓜ️ 微软服务`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=🍎 苹果服务`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=🎯 全球直连`select`[]🚀 节点选择`[]DIRECT`.*`[]♻️ 自动选择
custom_proxy_group=🛑 广告拦截`select`[]REJECT`[]🎯 全球直连`.*
custom_proxy_group=🎶 网易音乐`select`[]🚀 节点选择`[]🎯 全球直连`.*`[]♻️ 自动选择`(网易|音乐|解锁|Music|NetEase)
custom_proxy_group=🎮 游戏平台`select`[]🚀 节点选择`[]🎯 全球直连`.*
custom_proxy_group=💬 OpenAi`select`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=🍃 应用净化`select`[]REJECT`[]🎯 全球直连`.*
custom_proxy_group=🐟 漏网之鱼`select`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=🎥 奈飞节点`select`(NF|奈飞|解锁|Netflix|NETFLIX|Media)
custom_proxy_group=🎥 奈飞视频`select`[]🎥 奈飞节点`[]🚀 节点选择`[]♻️ 自动选择`[]🎯 全球直连`.*
custom_proxy_group=📺 巴哈姆特`select`[]🚀 节点选择`[]🎯 全球直连`.*
;设置分组标志位

enable_rule_generator=true
overwrite_original_rules=true
;clash_rule_base=https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/GeneralClashConfig.yml
;luck
~~~
