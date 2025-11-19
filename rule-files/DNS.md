🚀 2025最新版 | 国内外最全免费加密DNS（DoH/DoT）清单，提速、隐私、防劫持，一站搞定！收藏这一篇就够了。
📬 关注「索引目录」服务号，获取更多干货。

##🧠 为什么要用加密DNS？
传统DNS请求是明文的，意味着：

任何中间节点（ISP、公共Wi-Fi）都能看到你访问的网站；
甚至可能被DNS劫持，跳到假网站；
还会被部分运营商用来精准广告追踪。

##🔒 DoH（DNS over HTTPS） 和 DoT（DNS over TLS） 能将查询加密：
#防止监听与篡改；
#提升解析速度；
#保护隐私安全。

📊 加密DNS速览表
协议	名称	            默认端口	  特点
DoT	DNS over TLS	  853	      系统级加密，适合Android 9+、路由器
DoH	DNS over HTTPS	443	      穿透力强，浏览器兼容好

🇨🇳 国内主流公共DNS服务
🏆 阿里公共DNS
适用场景：国内主用首选，稳定、快速、隐私友好。

IPv4：223.5.5.5 / 223.6.6.6
IPv6：2400:3200::1 / 2400:3200:baba::1
DoH：https://dns.alidns.com/dns-query
DoT：dns.alidns.com
亮点：国内节点多、低延迟，企业与家庭通用。

⚡ 腾讯 DNSPod 公共DNS
适用场景：隐私保护强，支持国密算法。

IPv4：119.29.29.29 / 1.12.12.12 / 120.53.53.53
IPv6：2402:4e00::
DoH：502 Bad Gateway
国密DoH：https://sm2.doh.pub/dns-query
DoT：dot.pub
亮点：国密支持、安全等级高，兼容性强。

💡 百度公共DNS
IPv4：180.76.76.76
IPv6：2400:da00::6666
亮点：国内节点响应快，基础用户适用。

🛡️ 360公共DNS
电信/移动IPv4：101.226.4.6 / 218.30.118.6
联通IPv4：123.125.81.6 / 140.207.198.6
DoH：https://doh.360.cn
DoT：http://dot.360.cn
亮点：多线路优化，安全防护较强。

🧩 CNNIC DNS
IPv4：1.2.4.8 / 210.2.4.8
IPv6：2001:dc7:1000::1
亮点：中国互联网络信息中心官方节点，权威可靠。

🌈 台湾 Quad 101 (TWNIC)
IPv4：101.101.101.101 / 101.102.103.104
IPv6：2001:de4::101 / 2001:de4::102
DoH：https://dns.twnic.tw/dns-query
亮点：适合台港澳及东南亚用户，响应速度优。

🌍 国际主流加密DNS服务
🧠 Google Public DNS
IPv4：8.8.8.8 / 8.8.4.4
IPv6：2001:4860:4860::8888 / 2001:4860:4860::8844
DoH：https://dns.google/dns-query
DoT：dns.google
亮点：全球可靠，CDN智能路由，开发者首选。

⚙️ Cloudflare 公共DNS
IPv4：1.1.1.1 / 1.0.0.1
IPv6：2606:4700:4700::1111 / 2606:4700:4700::1001
DoH：https://cloudflare-dns.com/dns-query
DoT：one.one.one.one
亮点：速度全球第一，零日志，隐私保护极佳。

🔰 DNS.SB 公共DNS
IPv4：185.222.222.222 / 45.11.45.11
IPv6：2a09:: / 2a11::
DoH：https://doh.sb/dns-query
DoT：dot.sb
亮点：开源项目支持，提供多个节点（含香港）。

香港节点示例：
👉 https://hk-hkg.doh.sb/dns-query

🧩 AdGuard 公共DNS
默认过滤广告：94.140.14.14 / 94.140.15.15
无过滤：94.140.14.140 / 94.140.14.141
家庭保护：94.140.14.15 / 94.140.15.16
DoH：
https://dns.adguard.com/dns-query
https://dns-family.adguard.com/dns-query
https://dns-unfiltered.adguard.com/dns-query

DoT：
dns.adguard.com
dns-family.adguard.com
dns-unfiltered.adguard.com
亮点：拦截广告与追踪器，适合家庭与办公网络。

🛰️ OpenDNS (Cisco)
IPv4：208.67.222.222 / 208.67.220.220
IPv6：2620:0:ccc::2 / 2620:0:ccd::2
DoH：https://doh.opendns.com/dns-query
DoT：dns.umbrella.com
亮点：企业级安全防护，支持家庭过滤（FamilyShield）。

🧩 IBM Quad9 DNS
安全版 IPv4：9.9.9.9 / 149.112.112.112
安全版 IPv6：2620:fe::fe / 2620:fe::fe:9
DoH：https://dns.quad9.net/dns-query
DoT：dns.quad9.net
亮点：默认屏蔽恶意域名，隐私友好，无商业追踪。
附加版本：

无过滤版：9.9.9.10 / https://dns10.quad9.net/dns-query
ECS保护版：9.9.9.11 / https://dns11.quad9.net/dns-query

🧭 实用推荐榜单


场景	推荐DNS	理由
国内极速解析	阿里DNS	节点多，延迟低
隐私防追踪	Quad9 / AdGuard	拦截恶意与广告域名
国际访问优化	Cloudflare	全球CDN，速度稳定
家庭保护过滤	AdGuard Family / OpenDNS Family	屏蔽成人与广告内容
开发调试/跨境办公	Google DNS / Cloudflare	全球兼容性高


⚙️ 快速配置示例
Android 9+ / Windows 11
系统 → 网络设置 → 高级 → 私有DNS
填入：dns.alidns.com 或 dns.google

路由器 (OpenWRT)
/etc/config/network 添加：

option dns '1.1.1.1 8.8.8.8'
或启用 DoT 模式。

🧩 总结
在这个隐私被“标签化”的时代，加密DNS是你最简单、最有效的网络护盾。
选一个可靠的DNS，你的网络就能更快、更干净、更安全。

更新国内DoT列表如下：
tls.danqingximeng.top
dot.liweibin.com
alexander1995.top
whd.oder1988.cn
dot.yuanbaicai.vip
dns.clstudy.cn
dns.worthstudy.cn
tls.yu17.net（MaxMind地址库显示非国内）
cenxt.cn
dot.pub
dot.dns.pub
dot.sagez.cn
dot.onedns.net
101.198.198.198（MaxMind地址库显示该地址在境外）
tls.yuanbaicai.vip
dns.alidns.com
n.360.cn（MaxMind地址库显示对应地址在国外）
tls.dot.360.net

部分国内DoH列表：
v6.n.360.net/dns-query
v6.n.360.net/dns
tls.doh.pub/dns-query
doh.360.cn/dns-query
doh-pure.doh.pub/dns-query
doh.pub/dns-query
dot.onedns.net/dns-query
sm2.dns.pub/dns-query
tls.gemingyu.top/dns-query
dns.alidns.com/dns-query
doh.360.cn/doh
doh.qiaoba.online/dns-query
dns.worthstudy.cn/dns-query
dns.qiaoba.online/dns-query
