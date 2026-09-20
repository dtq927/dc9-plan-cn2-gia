# 搬瓦工 The DC9 Plan：年付38美元拿下CN2 GIA线路，配置、库存与购买避坑一次讲清

搜“搬瓦工 The DC9 Plan”的人，多半是刷到了这个名字听起来有点特别的套餐：年付38美元，1核768M，却挂着DC9 CN2 GIA机房。核心疑问无非几个——它到底值不值、现在还有没有货、和小几百美元的CN2 GIA-E套餐差在哪。这篇文章把这几个问题一次讲完，价格和套餐信息都基于官方购物车页面与多家长期跟踪搬瓦工的第三方站点核验。

## The DC9 Plan 是什么套餐

The DC9 Plan 是搬瓦工（BandwagonHost）在2024年4月15日上线的限量版套餐，归属“THE PLAN”系列产品。它发布的意义在于：搬瓦工时隔很久重新回到了低价位段，用38美元一年的价格提供DC9机房的CN2 GIA线路——这个价位此前只能买到CN2 GT甚至普通线路。

配置如下：

| 项目 | 参数 |
| --- | --- |
| CPU | 1核（限量约30%，采用积分策略） |
| 内存 | 768 MB |
| 硬盘 | 15 GB SSD |
| 月流量 | 750 GB |
| 带宽 | 1.5 Gbps |
| 机房 | 洛杉矶 DC9（USCA_9） |
| 价格 | $38.00/年 |

配置本身不高，甚至可以说偏低。768MB内存和15GB硬盘，跑个轻量服务、反代、小博客够用，想干重活就别指望了。它的卖点从来不在这套硬件，而在网络线路。

### 为什么大家盯着DC9机房

DC9是搬瓦工口碑最好的CN2 GIA机房之一。The DC9 Plan的线路走向是：去程电信走CN2 GIA，联通、移动直连；回程三网全部走CN2 GIA。对国内电信用户来说，这是花最少的钱拿到三网CN2 GIA回程的路径。

搬瓦工常规的CN2 GIA-E套餐入门价是$49.99/月，年付$169.99。The DC9 Plan把CN2 GIA的门槛压到了年付38美元，折合每月3美元出头——这就是它被抢的原因。HostHum等第三方测评实测后给出的结论也一致：性能偏弱，但网络速度符合预期，国内方向单线程轻松跑到100Mb/s以上，电信用户体验尤其好。

## 价格与优惠：38美元还能再便宜吗

$38.00/年是套餐原价。历史上在促销节点使用优惠码后，实际支付价约为**$35.42/年**（当时可用码为BWHCGLUKKB，折扣6.78%）。

关于优惠码，需要提醒的是现状：

- 搬瓦工在2025年11月双十一促销期间取消了全场常规优惠码，BWH3HYATVBJW、BWHCGLUKKB等老码此后陆续失效
- 2026年2月曾短暂上线优惠码NODESEEK2026（6.77%循环折扣），约两天后失效
- 截至2026年9月，没有长期稳定可用的公开优惠码

也就是说，如果你现在入手，按$38.00/年的原价准备预算即可；遇到大促节点（双十一、黑五）或官方临时放码，才有可能拿到35美元左右的实付价。结账前在购物车页面的促销码栏试一下当期码，没折扣就是没折扣，不用纠结。

## 现在还能买吗：限量版机制与库存

这里有一个必须先说的核验结果：**截至本文撰写时，The DC9 Plan在官方购物车显示缺货（Out of Stock）**。这不是意外——限量版套餐本来就是搬瓦工的常规操作。

限量版的规则是：上架一批，卖完就下架，等官方再次补货才会重新出现。The DC9 Plan自2024年4月首发后，在同年6月（618期间）补过货，之后长期处于售罄状态。想买的人基本靠等。

追踪补货有几个实用渠道：

1. 第三方库存监控站 stock.bwg.net，实时显示各限量套餐状态
2. 搬瓦工补货通知的TG频道和QQ群，补货时有推送
3. 直接访问套餐购买页面，缺货时页面会明确提示Out of Stock

补货没有固定时间表，历史上多出现在节假日促销前后。如果你不着急，可以先监控库存；如果急着用CN2 GIA线路，看下一节的替代方案更实际。

👉 [查看The DC9 Plan套餐页面（补货后可直接购买）](https://bandwagonhost.com/aff.php?aff=79616&pid=145)

## The DC9 Plan 适合谁，不适合谁

基于已核验的配置和第三方测评结论，判断其实很清楚。

适合的场景：

- 电信用户为主，需要三网CN2 GIA回程的轻量代理或中转
- 跑个低流量个人博客、静态站点、学习用的实验环境
- 对价格极度敏感，但线路质量不能妥协的用户

不适合的场景：

- 需要跑计算、数据库等CPU密集型任务——1核限量30%加上积分策略，性能在当下属于偏弱水平
- 需要大硬盘和大流量的应用，15GB/750GB都很紧
- 想后期换机房的用户——这一点下面单独说

## 两个购买前必须知道的限制

### 不支持迁移机房

常规搬瓦工套餐可以在KiwiVM面板里一键迁移到其他机房，这算搬瓦工的招牌功能之一。但The DC9 Plan不支持迁移，购买时锁定DC9机房。多方信源确认了这一点。如果你在意机房的灵活性，这个套餐不适合你；好在DC9本身就是搬瓦工最适合国内线路需求的机房之一，锁了也不算吃亏。

### 30天退款有条件

搬瓦工执行30天退款政策，但按官方ToS，需同时满足：订购不超过30天、账户无欠款且未违反ToS、该服务流量使用低于套餐限额的10%、账户历史无争议款项。满足条件后按原支付方式全额退款，同时账户下所有服务终止、数据被不可逆删除。简单说：买了之后头几天发现不合适，趁流量没用多少赶紧退，是来得及的。

付款方式支持支付宝、PayPal和信用卡，国内用户购买没有支付障碍。

## 搬瓦工在售套餐全对比

如果The DC9 Plan一直没货，或者你觉得配置不够，下面是搬瓦工官网当前展示的全部在售套餐（配置与价格来自官方购物车页面，以美元计价）。限量版套餐可能处于售罄状态，点击链接可查看实时库存。

| 系列/套餐 | 内存 | CPU | SSD | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **The DC9 Plan**（限量） | 768MB | 1核 | 15GB | 750GB | 1.5Gbps | $38.00/年 | [ 购买The DC9 Plan](https://bandwagonhost.com/aff.php?aff=79616&pid=145) |
| KVM PROMO 20G | 1GB | 2核 | 20GB | 1TB | 1Gbps | $49.99/年 | [ 查看KVM 20G](https://bandwagonhost.com/aff.php?aff=79616&pid=44) |
| KVM PROMO 40G | 2GB | 3核 | 40GB | 2TB | 1Gbps | $52.99/半年，$99.99/年 | [ 查看KVM 40G](https://bandwagonhost.com/aff.php?aff=79616&pid=45) |
| KVM PROMO 80G | 4GB | 4核 | 80GB | 3TB | 1Gbps | $19.99/月起，$199.99/年 | [ 查看KVM 80G](https://bandwagonhost.com/aff.php?aff=79616&pid=46) |
| KVM PROMO 160G | 8GB | 5核 | 160GB | 4TB | 1Gbps | $39.99/月起，$399.99/年 | [ 查看KVM 160G](https://bandwagonhost.com/aff.php?aff=79616&pid=47) |
| KVM PROMO 320G | 16GB | 6核 | 320GB | 5TB | 1Gbps | $79.99/月起，$799.99/年 | [ 查看KVM 320G](https://bandwagonhost.com/aff.php?aff=79616&pid=48) |
| KVM PROMO 480G | 24GB | 7核 | 480GB | 6TB | 1Gbps | $119.99/月起，$1199.99/年 | [ 查看KVM 480G](https://bandwagonhost.com/aff.php?aff=79616&pid=49) |
| CN2 GIA-E 20G | 1GB | 2核 | 20GB | 1TB | 2.5Gbps | $49.99/月，$169.99/年 | [ 购买CN2 GIA-E入门款](https://bandwagonhost.com/aff.php?aff=79616&pid=87) |
| CN2 GIA-E 40G | 2GB | 3核 | 40GB | 2TB | 2.5Gbps | $89.99/月，$299.99/年 | [ 查看CN2 GIA-E 40G](https://bandwagonhost.com/aff.php?aff=79616&pid=88) |
| CN2 GIA-E 80G | 4GB | 4核 | 80GB | 3TB | 2.5Gbps | $56.99/月，$549.99/年 | [ 查看CN2 GIA-E 80G](https://bandwagonhost.com/aff.php?aff=79616&pid=89) |
| CN2 GIA-E 160G | 8GB | 6核 | 160GB | 5TB | 5Gbps | $86.99/月，$879.99/年 | [ 查看CN2 GIA-E 160G](https://bandwagonhost.com/aff.php?aff=79616&pid=90) |
| CN2 GIA-E 320G | 16GB | 8核 | 320GB | 8TB | 5Gbps | $159.99/月，$1599.99/年 | [ 查看CN2 GIA-E 320G](https://bandwagonhost.com/aff.php?aff=79616&pid=91) |
| CN2 GIA-E 640G | 32GB | 10核 | 640GB | 10TB | 10Gbps | $289.99/月，$2759.99/年 | [ 查看CN2 GIA-E 640G](https://bandwagonhost.com/aff.php?aff=79616&pid=92) |
| CN2 GIA-E 1280G | 64GB | 12核 | 1280GB | 12TB | 10Gbps | $549.99/月，$5399.99/年 | [ 查看CN2 GIA-E 1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=93) |
| SLA 洛杉矶 20G | 1GB | 2核 | 20GB NVMe | 1TB | 2.5Gbps | $65.89/季，$239.99/年 | [ 查看SLA 20G](https://bandwagonhost.com/aff.php?aff=79616&pid=164) |
| SLA 洛杉矶 40G | 2GB | 3核 | 40GB NVMe | 2TB | 2.5Gbps | $116.99/季，$399.99/年 | [ 查看SLA 40G](https://bandwagonhost.com/aff.php?aff=79616&pid=165) |
| SLA 洛杉矶 80G | 4GB | 4核 | 80GB NVMe | 3TB | 2.5Gbps | $69.99/月起，$699.99/年 | [ 查看SLA 80G](https://bandwagonhost.com/aff.php?aff=79616&pid=166) |
| SLA 洛杉矶 160G | 8GB | 6核 | 160GB NVMe | 5TB | 5Gbps | $109.99/月起，$1099.99/年 | [ 查看SLA 160G](https://bandwagonhost.com/aff.php?aff=79616&pid=167) |
| SLA 洛杉矶 320G | 16GB | 8核 | 320GB NVMe | 8TB | 5Gbps | $199.99/月，$1999.99/年 | [ 查看SLA 320G](https://bandwagonhost.com/aff.php?aff=79616&pid=168) |
| SLA 洛杉矶 640G | 32GB | 10核 | 640GB NVMe | 10TB | 10Gbps | $369.99/月，$3699.99/年 | [ 查看SLA 640G](https://bandwagonhost.com/aff.php?aff=79616&pid=169) |
| SLA 洛杉矶 1280G | 64GB | 12核 | 1280GB NVMe | 12TB | 10Gbps | $699.99/月，$6999.99/年 | [ 查看SLA 1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=170) |
| 新加坡 CN2 GIA 40G | 2GB | 2核 | 40GB | 500GB | 1.5Gbps | $49.99/月，$499.99/年 | [ 查看新加坡40G](https://bandwagonhost.com/aff.php?aff=79616&pid=173) |
| 新加坡 CN2 GIA 80G | 4GB | 4核 | 80GB | 1TB | 1.5Gbps | $86.99/月，$869.99/年 | [ 查看新加坡80G](https://bandwagonhost.com/aff.php?aff=79616&pid=174) |
| 新加坡 CN2 GIA 160G | 8GB | 6核 | 160GB | 2TB | 2.5Gbps | $165.99/月，$1665.99/年 | [ 查看新加坡160G](https://bandwagonhost.com/aff.php?aff=79616&pid=175) |
| 新加坡 CN2 GIA 320G | 16GB | 8核 | 320GB | 4TB | 2.5Gbps | $329.99/月，$3199.00/年 | [ 查看新加坡320G](https://bandwagonhost.com/aff.php?aff=79616&pid=176) |
| 新加坡 CN2 GIA 640G | 32GB | 10核 | 640GB | 6TB | 5Gbps | $549.99/月，$5549.99/年 | [ 查看新加坡640G](https://bandwagonhost.com/aff.php?aff=79616&pid=177) |
| 新加坡 CN2 GIA 1280G | 64GB | 12核 | 1280GB | 8TB | 5Gbps | $1059.99/月，$10559.99/年 | [ 查看新加坡1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=178) |
| 大阪 CN2 GIA 40G | 2GB | 2核 | 40GB | 500GB | 1.5Gbps | $49.99/月，$499.99/年 | [ 查看大阪40G](https://bandwagonhost.com/aff.php?aff=79616&pid=134) |
| 大阪 CN2 GIA 80G | 4GB | 4核 | 80GB | 1TB | 1.5Gbps | $86.99/月，$869.99/年 | [ 查看大阪80G](https://bandwagonhost.com/aff.php?aff=79616&pid=135) |
| 大阪 CN2 GIA 160G | 8GB | 6核 | 160GB | 2TB | 1.5Gbps | $165.99/月，$1665.99/年 | [ 查看大阪160G](https://bandwagonhost.com/aff.php?aff=79616&pid=136) |
| 大阪 CN2 GIA 320G | 16GB | 8核 | 320GB | 4TB | 1.5Gbps | $329.99/月，$3279.99/年 | [ 查看大阪320G](https://bandwagonhost.com/aff.php?aff=79616&pid=137) |
| 大阪 CN2 GIA 640G | 32GB | 10核 | 640GB | 6TB | 1.5Gbps | $549.99/月，$5549.99/年 | [ 查看大阪640G](https://bandwagonhost.com/aff.php?aff=79616&pid=138) |
| 大阪 CN2 GIA 1280G | 64GB | 12核 | 1280GB | 8TB | 1.5Gbps | $1059.99/月，$10559.99/年 | [ 查看大阪1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=139) |
| 东京 CN2 GIA 40G | 2GB | 2核 | 40GB | 500GB | 1.2Gbps | $89.99/月，$899.99/年 | [ 查看东京40G](https://bandwagonhost.com/aff.php?aff=79616&pid=108) |
| 东京 CN2 GIA 80G | 4GB | 4核 | 80GB | 1TB | 1.2Gbps | $155.99/月，$1559.99/年 | [ 查看东京80G](https://bandwagonhost.com/aff.php?aff=79616&pid=109) |
| 东京 CN2 GIA 160G | 8GB | 6核 | 160GB | 2TB | 1.2Gbps | $299.99/月，$2999.99/年 | [ 查看东京160G](https://bandwagonhost.com/aff.php?aff=79616&pid=110) |
| 东京 CN2 GIA 320G | 16GB | 8核 | 320GB | 4TB | 1.2Gbps | $589.99/月，$5899.99/年 | [ 查看东京320G](https://bandwagonhost.com/aff.php?aff=79616&pid=111) |
| 东京 CN2 GIA 640G | 32GB | 10核 | 640GB | 6TB | 1.2Gbps | $989.99/月，$9989.99/年 | [ 查看东京640G](https://bandwagonhost.com/aff.php?aff=79616&pid=123) |
| 东京 CN2 GIA 1280G | 64GB | 12核 | 1280GB | 8TB | 1.2Gbps | $1889.99/月，$18989.99/年 | [ 查看东京1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=125) |
| 香港 CN2 GIA 40G | 2GB | 2核 | 40GB | 500GB | 1Gbps | $89.99/月，$899.99/年 | [ 查看香港40G](https://bandwagonhost.com/aff.php?aff=79616&pid=95) |
| 香港 CN2 GIA 80G | 4GB | 4核 | 80GB | 1TB | 1Gbps | $155.99/月，$1559.99/年 | [ 查看香港80G](https://bandwagonhost.com/aff.php?aff=79616&pid=96) |
| 香港 CN2 GIA 160G | 8GB | 6核 | 160GB | 2TB | 1Gbps | $299.99/月，$2999.99/年 | [ 查看香港160G](https://bandwagonhost.com/aff.php?aff=79616&pid=97) |
| 香港 CN2 GIA 320G | 16GB | 8核 | 320GB | 4TB | 1Gbps | $589.99/月，$5899.99/年 | [ 查看香港320G](https://bandwagonhost.com/aff.php?aff=79616&pid=98) |
| 香港 CN2 GIA 640G | 32GB | 10核 | 640GB | 6TB | 1Gbps | $989.99/月，$9989.99/年 | [ 查看香港640G](https://bandwagonhost.com/aff.php?aff=79616&pid=122) |
| 香港 CN2 GIA 1280G | 64GB | 12核 | 1280GB | 8TB | 1Gbps | $1889.99/月，$18989.99/年 | [ 查看香港1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=124) |
| 迪拜 ECOMMERCE 20G | 1GB | 2核 | 20GB | 500GB | 1Gbps | $19.99/月，$169.99/年 | [ 查看迪拜20G](https://bandwagonhost.com/aff.php?aff=79616&pid=114) |
| 迪拜 ECOMMERCE 40G | 2GB | 3核 | 40GB | 1TB | 1Gbps | $32.99/月，$299.99/年 | [ 查看迪拜40G](https://bandwagonhost.com/aff.php?aff=79616&pid=115) |
| 迪拜 ECOMMERCE 80G | 4GB | 4核 | 80GB | 2TB | 1Gbps | $56.99/月，$549.99/年 | [ 查看迪拜80G](https://bandwagonhost.com/aff.php?aff=79616&pid=116) |
| 迪拜 ECOMMERCE 160G | 8GB | 6核 | 160GB | 3TB | 1Gbps | $86.99/月，$879.99/年 | [ 查看迪拜160G](https://bandwagonhost.com/aff.php?aff=79616&pid=117) |
| 迪拜 ECOMMERCE 320G | 16GB | 8核 | 320GB | 4TB | 1Gbps | $159.99/月，$1599.99/年 | [ 查看迪拜320G](https://bandwagonhost.com/aff.php?aff=79616&pid=118) |
| 迪拜 ECOMMERCE 640G | 32GB | 10核 | 640GB | 5TB | 1Gbps | $289.99/月，$2759.99/年 | [ 查看迪拜640G](https://bandwagonhost.com/aff.php?aff=79616&pid=119) |
| 迪拜 ECOMMERCE 1280G | 64GB | 12核 | 1280GB | 6TB | 1Gbps | $549.99/月，$5399.99/年 | [ 查看迪拜1280G](https://bandwagonhost.com/aff.php?aff=79616&pid=120) |

几点读表提示：

- CN2 GIA-E系列可任选机房，包括DC6 CN2 GIA-E、DC9 CN2 GIA、东京、大阪、荷兰等，支持在KiwiVM面板内免费迁移，这是它与The DC9 Plan最大的差别之一
- KVM PROMO系列机房以普通线路为主，价格虽低但没有CN2 GIA，国内直连体验不在一个档次
- SLA洛杉矶系列主打99.99%在线率保障和NVMe硬盘，面向建站和电商场景，价格也最高
- 香港、东京、新加坡机房物理距离近，延迟低，但流量配额小、月付价格高，适合对延迟敏感的特定用途

如果只想要CN2 GIA线路而The DC9 Plan缺货，CN2 GIA-E 20G（年付$169.99）是最接近的常规替代，代价是价格翻了四倍多，换来的是可迁移机房、2.5Gbps带宽和1TB流量。

👉 [查看搬瓦工全部在售套餐与实时库存](https://bit.ly/BandwagonHost)

## 常见问题

**The DC9 Plan后续怎么续费？**

按原价$38.00/年续费。限量版套餐续费价与购买价一致，不会因为次年市场变化涨价。如果当期有可用优惠码，续费同样适用。

**768MB内存装什么系统合适？**

KiwiVM面板提供CentOS、Debian、Ubuntu、RockyLinux、AlmaLinux等模板，均可一键重装。768MB内存建议选Debian或AlmaLinux这类轻量发行版，避开重量级面板和数据库组合。

**流量用超了怎么办？**

超出750GB月流量后，按搬瓦工通用规则计费或限速，具体以KiwiVM面板内当前政策为准。对15GB硬盘、1核限量的配置来说，流量跑满的可能性不大。

**IP被墙了怎么办？**

该套餐不能通过迁移机房换IP，只能在KiwiVM面板内付费更换IP。如果在30天退款期内且流量使用低于10%，也可以直接按ToS申请退款，这是成本最低的处理方式。

## 总结：这笔钱该不该花

The DC9 Plan的逻辑很简单：你花的38美元，绝大部分买的是DC9机房的CN2 GIA线路，硬件只是捎带的。如果你的需求就是电信方向稳定、快速的轻量用途，它在搬瓦工全线乃至同类商家中都是价格最低的CN2 GIA方案之一，唯一的问题是缺货要等。如果你需要更好的性能、更大的存储或机房灵活性，加预算上CN2 GIA-E系列是更合理的选择。想清楚自己缺的是线路还是配置，选择就不难。
