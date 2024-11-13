---
title: PC Direct
description:
type: “Docs”
tip: 顶部栏固定格式请勿删除,description为文章描述，不填时将截取内容最前一段文字
---
# 一种不同的设置方法
无论您是出于个人还是专业目的使用 ZimaOS 设备，了解如何通过各种网络进行连接至关重要。本指南将涵盖三种主要的网络连接类型：直接连接、局域网（LAN）和广域网（WAN）。每种方法都有独特的好处和应用，确保您在家中或外出时都能无缝访问和管理您的数据。

本文旨在理解不同网络下的连接。

## 直接连接
![](https://manage.icewhale.io/api/static/docs/1726131286208_image.png)

直接连接非常适合快速和简单的设置，提供了一种快速和安全的方式来连接设备，无需更广泛的网络。这种方法非常适合文件传输或使用需要高速访问的特定应用程序。

{% note warn Tips: %}
如果您在使用 Thunderbolt 时遇到任何问题，可以在 [这里](/zimacube/Connecting-ZimaCube-via-Thunderbolt.html) 获取更多详细信息
{% endnote %}

**您需要的：**

* 网络电缆或用于高速连接的 Thunderbolt 电缆

* ZimaOS 设备（ZimaCube Pro 配备 Thunderbolt）和客户端设备（笔记本电脑、台式 PC 等）

步骤：

1. **建立连接：** 使用标准网络电缆将客户端设备直接连接到 ZimaOS 设备，或利用 Thunderbolt 电缆（ZimaCube Pro 用户）实现最高 20G 的速度，非常适合处理高要求任务。

2. **网络配置：** IP 通过自动配置功能分配。它将是 169.254.x.x 这样的格式。
![](https://manage.icewhale.io/api/static/docs/1726131302533_image.png)

3. **这意味着您的连接成功：** 屏幕上显示的 IP 如 169.254.x.x 表示直接连接成功。
![](https://manage.icewhale.io/api/static/docs/1726131333502_image.png)

**应用示例和用例：** 利用高速连接，特别适合视频编辑或其他需要大量带宽的任务。它非常适合低延迟和高速数据传输至关重要的场景。


## 局域网（LAN）连接
![](https://manage.icewhale.io/api/static/docs/1726131416246_image.png)

通过局域网连接 ZimaOS 设备提供了一个强大且稳定的网络环境，非常适合需要有效共享资源的家庭或小型企业，其中多个设备需要共享资源。

**您需要的：**

* 路由器或网络交换机

* ZimaOS 设备（ZimaCube Pro 配备 10G NIC）和客户端设备（手机、笔记本电脑、台式 PC 等）

**步骤：**

1. **连接到网络：** 将 ZimaOS 设备和其他客户端设备连接到路由器或交换机。

2. **网络配置：** 检查所有设备是否在同一子网，并能相互通信。它会是类似 192.168.x.x 或 10.0.x.x 的格式，具体取决于您的 LAN 配置。您可以手动分配静态 IP 地址以确保设备一致性，或依赖 DHCP 进行自动分配。

3. **这意味着您的连接成功：** 屏幕上显示的 IP 如 192.168.x.x 表示 LAN 连接成功。LAN IP 取决于您的 LAN 配置。
![](https://manage.icewhale.io/api/static/docs/1726131462130_image.png)

**应用示例和用例：** 在设备之间流式传输和管理媒体内容，享受无缝访问您的库。最适合需要可靠和快速本地网络访问的环境，例如媒体服务器或共享文件存储。
![](https://manage.icewhale.io/api/static/docs/1726131473384_image.png)

## 哪一个会被选择？
当您同时拥有直接连接和 LAN 连接时，您会选择哪一个？
![](https://manage.icewhale.io/api/static/docs/1726131488677_image.png)

如果您已阅读我们的教程 4 关于 SAMBA，这是体验 NAS 的一种重要方式，您可能会掌握将 NAS 驱动器挂载到客户端设备的正确方法。要注意的要点有两个规则：

1. 使用 Zima 应用时优先选择 Thunderbolt。

2. 您可以通过手动挂载文件夹通过相应的 IP 来选择特定的连接。
![](https://manage.icewhale.io/api/static/docs/1726131521116_image.png)

## 广域网（WAN）连接
![](https://manage.icewhale.io/api/static/docs/1726131531121_image.png)

WAN 连接使您能够远程访问您的 ZimaOS 设备，允许您从任何具有 Internet 连接的地方进行连接。这对于远程工作或在旅行过程中访问个人数据特别有用。

为了增强安全性和访问便利性，我们使用 Zerotier 创建虚拟网络，简化连接过程。
![](https://manage.icewhale.io/api/static/docs/1726131539225_image.png)

**您需要的：**

* 每个设备的互联网连接

* 获取 ZimaOS 设备的远程登录 ID。此 ID 是 Zerotier ID，您可以从 ZimaOS 仪表板 → 网络 → 远程登录获取。
![](https://manage.icewhale.io/api/static/docs/1726131699787_image.png)

* 对于您的 Windows/Mac，需要一个 [Zima APP](https://find.zimaspace.com) 5（集成了 Zerotier）。
**步骤：**

1. **建立连接：** 在您的 Windows/Mac 上下载并启动 Zima 应用。点击系统任务栏右侧的应用图标并选择通过网络 ID 连接。之后，您可能需要输入您的 WebUI 用户名和密码。
![](https://manage.icewhale.io/api/static/docs/1726131911735_image.png)

2. **网络配置：** 基本上，您无需进一步的网络配置，因为 Zima 应用已经为您完成了这些。

3. **这意味着您的连接成功：** 您将导航到 ZimaOS 的仪表板。
![](https://manage.icewhale.io/api/static/docs/1726131933130_image.png)

**应用示例和用例：** 使用 WAN 连接安全地访问关键文件或在紧急情况下管理设备。它非常适合需要远程管理或访问其 ZimaOS 设备的用户，确保重要数据的持续可用性。
![](https://manage.icewhale.io/api/static/docs/1726131946008_image.png)

可选：可以配置动态 DNS 的公共 IP 地址作为选项，因为您可以通过域名直接访问您的设备。

## 结论
无论您的需求是什么，ZimaOS 提供灵活强大的连接选项以适应任何情况。从高速直接连接到方便的 WAN 远程访问，您可以轻松管理您的设备和数据。处理 WAN 连接时，始终考虑安全措施，以保护您的信息并保持顺利运行。

如果您在使用过程中遇到任何问题，请随时告知我们。您也可以加入我们的社区和 Discord，与大家讨论有关 ZimaCube 和 ZimaOS 的更多内容。我们期待您的反馈！