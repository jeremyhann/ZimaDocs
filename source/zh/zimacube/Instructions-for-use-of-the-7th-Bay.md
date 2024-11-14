---
title: 第七个硬盘位的使用 
description:
type: “Docs”
tip: 顶部栏固定格式请勿删除,description为文章描述，不填时将截取内容最前一段文字
---
# 安装和移除第七个硬盘位
## 准备工作:
确保ZimaCube已关闭电源并拔掉插头。
准备要安装的硬盘。
## 具体步骤:
步骤1: 拆下机箱前面板。
![](https://manage.icewhale.io/api/static/docs/1722418820491_image.png)
步骤2: 移除第六个硬盘位。
![](https://manage.icewhale.io/api/static/docs/1722418858886_image.png)
步骤3: 逆时针旋转，拧下固定第七个驱动器的螺丝。
![](https://manage.icewhale.io/api/static/docs/1722418913222_image.png)
步骤4: 移除第七个硬盘位。
![](https://manage.icewhale.io/api/static/docs/1722418964759_image.png)
![](https://manage.icewhale.io/api/static/docs/1722418974044_image.png)
步骤5: 自由安装SSD到第七个硬盘位上。
![](https://manage.icewhale.io/api/static/docs/1722419028169_image.png)
步骤6: 将第七个硬盘位推入正确位置，顺时针拧紧螺丝。
![](https://manage.icewhale.io/api/static/docs/1722419069919_image.png)

# 如何升级ZimaCube第七个硬盘位的固件
*为了防止esp32在OTA（无线更新）中失败，这里引入了一种有线更新方法。*
## 三步解决方案
1. 连接WiFi
用电脑连接WiFi
名称: "ZimaCube"
密码: "homecloud"
2. 输入URL
在浏览器中输入: 172.16.1.1
3. 上传固件
[https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link](https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link)

## 备用计划

**更新前准备**
- 电脑
- Type-C数据线
- 磁盘7
- 下载并解压缩压缩包
[https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link](https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link)

**开始更新**
3.1 使用Type-C数据线将电脑连接到第七个磁盘芯片上的Type-C接口
3.2 在电脑上打开链接 [espressif.github.io](espressif.github.io)
3.3 点击“连接”
![](https://manage.icewhale.io/api/static/docs/1730360675989_image.png)

3.4 选择串口进行连接
![](https://manage.icewhale.io/api/static/docs/1730360689217_image.png)

3.5 点击“DIY”
![](https://manage.icewhale.io/api/static/docs/1730360715808_image.png)

3.6 点击“添加文件”两次
![](https://manage.icewhale.io/api/static/docs/1730360989529_image.png)

3.7 更改烧录地址并选择文件
*具体烧录地址如图所示，依次选择解压后的三个文件*
![](https://manage.icewhale.io/api/static/docs/1730360997291_image.png)

3.8 点击“程序”开始烧录
![](https://manage.icewhale.io/api/static/docs/1730361017895_image.png)

3.9 烧录完成，按下RST重置按钮，固件成功更新。