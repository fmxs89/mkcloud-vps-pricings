# mkcloud vps：跨境专线VPS怎么选？广港/沪日/沪美全套餐价格与优惠码完整指南

搜 mkcloud vps 的人，多半已经过了“什么是VPS”的阶段。真正想搞清楚的是三件事：这家号称做IEPL/IPLC专线的商家靠不靠谱、全套餐到底什么价、和自己要做的业务匹不匹配。这篇文章就按这个顺序把事情说清楚，价格和套餐信息都对照了官网商店和第三方测评数据，最后附上购买前必须知道的几条规则。

## mkcloud vps 是什么？先分清“专线 VPS”和普通 VPS

Mkcloud 是 2023 年起家的国人商家，定位很窄：只做合规的跨境电商专线服务器。产品线全走 IEPL、IPLC 和 IX 三类跨境专线，入口在广州、上海、福建，出口覆盖香港、日本、美国，另有一个上海本地 CN2 产品。付款目前只支持支付宝，下单前需要国内身份信息实名认证。

它和普通 VPS 的核心差别在网络路径上。普通 VPS 走公网，晚高峰绕路、丢包都很常见；专线产品走的是点对点的专用线路，官方给的端内参考延迟是：广港 IEPL 约 1~2ms，沪日 IPLC 约 25~28ms，沪美 IPLC 约 124~134ms。

另一个容易混淆的概念是“单端双 IP”。每台专线 VPS 分配一个独立入口 IP 和一个独立出口 IP：你用远程桌面或 SSH 连入口，业务流量从出口 IP 向外发起。出口端不接受外部连入，所以这套架构天生不适合建站、收邮件这类需要“被访问”的业务——它是给店铺后台操作、素材上传、直播推流、授权 API 调用这类“主动出站”的业务准备的。

## 全套餐价格与购买入口

先把结论放在前面：入门门槛是深港/沪港 IXP 专线的 158 元/月，主流的广港 IEPL 从 500GB 档的 198 元/月起，上海 CN2 属于稀缺资源型产品，4500 元/月起。下面两张表覆盖了官网当前在售的主要档位。

**流量计费套餐（双向流量统计）：**

| 套餐 | CPU/内存/硬盘 | 峰值带宽 | 月流量 | 端内延迟 | 月价 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 深港IXP 2TB | 2核4G/40GB | 200Mbps | 2TB | 约1~2ms | ¥158 | [ 查看深港IX现价](https://bit.ly/MKCLoud) |
| 沪日IX(上云互联) 1TB | 2核4G/40GB | 200Mbps | 1TB | 25~28ms | ¥166 | [ 选购沪日IX套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/cloud-jp-sh) |
| 广港IEPL 500GB | 1核2G/20GB | 150Mbps | 500GB | 1~2ms | ¥198 | [ 选购广港IEPL套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/gz-hk-sh) |
| 沪美IPLC 100GB | 1核2G/20GB | 150Mbps | 100GB | 124~134ms | ¥198 | [ 查看沪美IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-us-sh) |
| 沪美IXP 1TB | 2核4G/40GB | 200Mbps | 1TB | 124~134ms | ¥266 | [ 查看沪美IXP现价](https://bit.ly/MKCLoud) |
| 沪美IPLC 500GB | 1核2G/20GB | 150Mbps | 500GB | 124~134ms | ¥258 | [ 查看沪美IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-us-sh) |
| 沪日IX(上云互联) 2TB | 2核4G/40GB | 300Mbps | 2TB | 25~28ms | ¥268 | [ 选购沪日IX套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/cloud-jp-sh) |
| 沪港IPLC 共享1024GB | 1核2G/20GB | 200Mbps | 1024GB | 约21ms | ¥288 | [ 查看沪港IPLC现价](https://bit.ly/MKCLoud) |
| 沪日IPLC 500GB | 1核2G/20GB | 150Mbps | 500GB | 25~28ms | ¥228 | [ 查看沪日IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-jp-sh) |
| 广港IEPL 1TB | 1核2G/20GB | 200Mbps | 1TB | 1~2ms | ¥358 | [ 选购广港IEPL套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/gz-hk-sh) |
| 沪日IPLC 1TB | 1核2G/20GB | 200Mbps | 1TB | 25~28ms | ¥358 | [ 查看沪日IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-jp-sh) |
| 沪日IX(上云互联) 3TB | 2核4G/40GB | 500Mbps | 3TB | 25~28ms | ¥358 | [ 选购沪日IX套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/cloud-jp-sh) |
| 沪美IXP 2TB | 2核4G/40GB | 200Mbps | 2TB | 124~134ms | ¥430 | [ 查看沪美IXP现价](https://bit.ly/MKCLoud) |
| 沪美IPLC 1TB | 1核2G/20GB | 200Mbps | 1TB | 124~134ms | ¥428 | [ 查看沪美IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-us-sh) |
| 广港IEPL 2TB | 2核4G/40GB | 300Mbps | 2TB | 1~2ms | ¥568 | [ 选购广港IEPL套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/gz-hk-sh) |
| 沪日IPLC 2TB | 2核4G/40GB | 300Mbps | 2TB | 25~28ms | ¥568 | [ 查看沪日IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-jp-sh) |
| 沪美IPLC 2TB | 2核4G/40GB | 300Mbps | 2TB | 124~134ms | ¥698 | [ 查看沪美IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-us-sh) |
| 沪日IX(上云互联) 6TB | 4核8G/40GB | 1Gbps | 6TB | 25~28ms | ¥688 | [ 选购沪日IX套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/cloud-jp-sh) |
| 沪美IPLC 4TB | 2核4G/40GB | 300Mbps | 4TB | 124~134ms | ¥1258 | [ 查看沪美IPLC套餐](https://www.mkcloud.net/aff.php?aff=390&url=https://www.mkcloud.net/index.php/store/sh-us-sh) |
| 深港IX 5TB大流量版 | 4核8G/40GB | 1Gbps | 5TB | 约1~2ms | ¥368 | [ 查看深港IX现价](https://bit.ly/MKCLoud) |
| 上海CN2(动态IP双线) | 独享型 | — | — | — | ¥4500 | [ 前往商店查看上海CN2](https://bit.ly/MKCLoud) |

两点说明。第一，各线路还有 10TB、20TB 甚至 30TB/50TB 的更高档位，以及沪美独享带宽（5M 档 850 元/月起）和上云互联独享带宽（100M 档 1600 元/月起）产品，这里没占篇幅，购买前建议在商店里核对。第二，价格存在时间差：官网首页目前给广港 IEPL 标的是“358 元/月起”，而第三方测评和商店订单页展示的 500GB 档是 198 元/月。这种出入说明套餐和价格在滚动调整，下单价以结算页实时显示为准。

买之前想先看全场价格再决策的，可以[👉 进入 Mkcloud 商店对比各线路档位](https://bit.ly/MKCLoud)。

## 分线路点评：按业务方向选，别按价格选

**广港 IEPL：华南出海的主力线。** 入口可选八线动态 BGP 或电信/移动/联通/三线，端内延迟 1~2ms，第三方实测广州入口 TCP ping 电信约 34ms、联通 33ms、移动 38ms。对 TikTok 直播推流、店铺后台操作这种要求链路稳的业务，这条线的价格在同类专线里不算离谱。

**沪日方向：IPLC 和 IX 是两种玩法。** 沪日 IPLC 入口是 UCloud BGP/电信，直接就能用；沪日 IX(上云互联)便宜一截，但只允许云厂 BGP 网络连入——目前上海入口支持阿里云、腾讯云、百度云国内全网，以及火山云、华为云、UCloud 华东。你自己得先有一台符合范围的云机做前置。做亚马逊日本站、乐天的，25ms 出口延迟已经接近本地操作手感。

**沪美方向：给美区业务兜底。** 沪美 IPLC 延迟 124~134ms，这是物理距离决定的，没什么奇迹可言。它适合美区电商后台、独立站管理和广告投放管理这类对“稳”敏感、对“快”不极端敏感的场景。同方向还有沪美 IXP 流量计费套餐，1TB 档 266 元/月，价格更低，同样需要云厂前置接入。

**香港方向：深港 IX 和沪港 IPLC 门槛不同。** 深港 IX 走深圳入口+腾讯广州八线 BGP，端内 1~2ms，158 元/月的 2TB 档是全站最低入门价，但同样只允许云厂 BGP 网络连入。沪港 IPLC 是传统直连产品，288 元/月的共享档不需要云前置。香港出口走的 BGP 生态接入了 PCCWG、NTT、Cogent、Lumen 等多家，并且有到 Google、Cloudflare 的私有 PNI 互联。

**上海 CN2：不是给普通用户准备的。** 4500 元/月起步，上海动态联通入口、上海电信 CN2 出口，属于动态 IP 双线的国内优化产品。官方知识库特别提醒：不能仅凭"CN2"名称就认定它是全程 CN2 GIA，也别把它当海外出口用。

## 优惠码与省钱方法

Mkcloud 的优惠体系比多数商家复杂一点，下单时可以在购物车“优惠券码”栏直接输入验证：

- **MK-8.8**：流量计费产品全场 88 折循环折扣。所谓“循环”，是每次续费都自动打折，不是只打首月。
- **MK-7.8**：独享带宽产品首月 78 折。
- **MK-IEPL-WELCOME / MK-IPLC-WELCOME**：IEPL 和 IPLC 产品线各自的 9 折循环码（最低配套餐通常不可用）。
- **IXCLOUD**：部分上云互联 IX 产品 6.9 折，历史上的使用案例是 2TB 档折后 184.92 元/月。

需要注意的是，这些码在官方知识库里出现过“仅活动期内有效”的标注，也有 2026 年的第三方汇总把它们列为在用。最稳的做法是下单时挨个试一遍，系统会自动匹配最优惠的价格，试不出折就是失效了。另外，官网知识库的推广联盟说明中写明的返佣比例是 10%，部分节庆活动会叠加邀请奖励，介意价格的话可以关注 Telegram 通知群的动态。

## 实名、退款与售后：下单前必须知道的几条规则

这部分直接决定你会不会后悔，值得单独一段。

> IPLC/IEPL 产品需要中国手机号+身份证+姓名一致性实名认证；专线产品采用省级白名单机制，只能从你绑定的省份 IP 连入，省份可随时切换；仅支持质量问题退款，需要提交具体延迟、速度数据作为证据，开通后不支持更换地域。

退款之外还有几条容易踩坑的规则：流量按上行+下行双向统计，用完直接暂停（可自助购买流量重置或工单补差价升级）；共享带宽标注的是峰值，不保证持续跑满；升降级都要走工单，降级到更低价套餐时差价不退；产品不提供快照和备份，重要数据自己安排。支付方式目前只有支付宝。

## 第三方测评数据怎么说

第三方测评站 vps.dance 公布过一次广港 IEPL 的完整测试：AMD EPYC 平台、KVM 虚拟化，香港出口单线程国际测速在 130Mbps 上下（对应 150Mbps 峰值档），Cloudflare 延迟 5.7ms，出口 IP 归属 Nearoute（AS147293），scamalytics 欺诈评分 0/100。猎者出海的评测同样给出了 scamalytics 欺诈值为 0 的结果，工单响应在 12~24 小时内，但在线客服高峰期经常忙碌。两份数据指向同一个结论：IP 质量是这个产品的主要卖点之一，适合 eBay、Shopee、TikTok 这类对 IP 信任度敏感的业务；售后则靠工单，别指望即时在线客服。

## 适合谁买，谁别碰

适合的情况很明确：跨境电商店铺运营需要固定干净的出口 IP；TikTok 直播推流要稳定低延迟的华南线路；日本站、美区业务需要固定环境管理后台；或者企业要给授权 API 和海外 SaaS 做合规出站。这些场景下，它 158~358 元/月的价格对应的是专线级链路，月付机制也让试错成本可控。

不适合的情况同样明确：想建网站做支付回调的（出口不支持入站连接）；想拿来做机场或共享代理的（官方明确禁止，白名单机制也会拦住）；想找十几块钱一个月的玩具机的（这不是那个价位的产品）；以及没有国内身份信息、无法实名认证的海外用户。

## 常见问题

**mkcloud vps 需要实名吗？** 需要。IPLC/IEPL 产品要求中国身份信息实名认证，且用途需合规。

**能退款吗？** 仅质量问题可退，需在工单里提交具体的延迟和速度证据，开通后不支持换地域。

**配置怎么选？** 官方套餐起步就是 1核2G/20GB，硬件本身不是这类产品的重点，预算应该优先给流量档位。拿不准档位时按一个月真实业务流量乘 1.2 倍估，超量是可以补差价升级的。

**广港、沪日、深港到底先选哪个？** 业务在华南或对延迟最敏感，选广港 IEPL；人在上海周边或做日本市场，选沪日；预算紧、手上有阿里云/腾讯云机器的，深港 IX 或沪日 IX 的上云互联产品性价比最高。拿定主意后从[👉 Mkcloud 全线商店入口](https://bit.ly/MKCLoud)进去按档位下单即可，开通资料里的入口地址、端口和绑定省份记得先核对再连接。
