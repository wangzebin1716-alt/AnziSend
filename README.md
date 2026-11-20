# AnziSend

**在电脑与手机之间收发文件。局域网内可以离线直传，身处不同网络时可以用身份码尝试连接。**

AnziSend 可以在家里传照片、在办公室交接大文件，也可以和校园网里的同学互传资料。两台设备在内网中能互相访问时，即使连着不同的 Wi‑Fi，或一台接网线，也能直接传输。临时借用一台电脑时，可以打开网页版收发文件。Windows 版还提供本地 AI，帮你分类整理收到的文件。

[官网下载](https://www.anzisend.cn/#download) · [打开网页版](https://api.anzisend.cn/connect) · [GitHub Releases](https://github.com/wangzebin1716-alt/AnziSend/releases)

## 选一种传输方式

| 你的场景 | 用什么方式 | 开始前确认 |
| --- | --- | --- |
| 家里没接互联网，或在同一企业、校园的内网里 | 软件内局域网直传 | 两台设备能在内网互访。访客 Wi‑Fi 或设备隔离可能拦截连接。 |
| 一台在企业网，另一台在校园网，或两台设备在不同城市 | 用 12 位身份码查找对方，核对身份后尝试跨网直连 | 双方在线，使用支持跨网直连的版本。需要可达的 IPv6 连接，或成功建立 IPv4 打洞连接。 |
| 临时借用电脑，需要从浏览器收发 | 打开网页版，连接身份服务，选择已核对的在线好友 | 浏览器有自己的设备身份。能否传输取决于双方网络。 |

### 局域网直传

1. 在两台设备上打开 AnziSend，让设备接入可互访的内网。
2. 在设备列表找到接收方，核对设备身份。
3. 选择文件或文件夹发送。接收方确认后，可以查看传输进度。桌面版可设置接收目录、查看接收记录和续传大文件。

### 跨网络直连

1. 双方打开 AnziSend 并保持在线。请对方提供 12 位设备身份码。
2. 在「身份码与好友」中查找对方。核对设备指纹并完成好友确认。
3. 从在线设备中选择对方并发送文件。

跨网络直连目前处于测试阶段。身份服务用于查找设备和协调连接，文件传输依赖设备间的直连。目前没有文件中继。运营商 NAT、企业防火墙、VPN 或手机热点都可能影响连接，出现「搜得到对方，但文件发不出去」时，可以检查双方网络是否允许直连。

### 网页版收发

打开网页版，点击「连接」，再用设备名称或身份码查找对方。核对身份并完成好友确认后，在「发送文件」选择在线好友。收到的文件可从「收到的文件」下载。网页版的身份和浏览器中保存的文件可能会随网站数据一起清除，收到重要文件后请及时下载。

## 设备查找、消息与本地 AI

- **设备查找与隐私**。网页版首次连接、软件从 build131 起首次建立身份查找资料时，默认允许通过设备名称和身份码查找，无需先点保存。已有设备保存的查找设置继续生效。软件里可以在「身份码与好友」关闭查找。网页版取消勾选后，点击「保存名称与查找设置」即可。
- **文件、文件夹与消息**。软件内可拖入文件或文件夹发送，也能给已连接的设备发消息。Windows 版使用当前系统账户加密保存聊天记录和草稿。
- **Windows 本地 AI**。可在本机分类整理收到的文件。轻量版按需下载模型，离线完整版随安装包附带模型，适合需要在无互联网环境中使用 AI 的场景。

## 平台与下载

以下为 **AnziSend 1.18.3-build131 公开测试版**的下载包。[查看版本说明](https://github.com/wangzebin1716-alt/AnziSend/releases/tag/v1.18.3-build131)

| 平台 | 安装包 | 说明 |
| --- | --- | --- |
| Windows x64 | [轻量版](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/AnziSend-1.18.3-build131-windows-x64-light-unsigned-setup.exe) · [离线 AI 完整版](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/AnziSend-1.18.3-build131-windows-x64-unsigned-setup.exe) | 两款均为未签名测试安装包。 |
| Android ARM64 | [签名 APK](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/AnziSend-1.18.3-build131-android-arm64-release.apk) | 适用于 ARM64 Android 设备。 |
| Linux x64 | [AppImage](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/AnziSend-1.18.3-build131-linux-x64.AppImage) | 适用于 x86‑64 Linux。 |
| macOS | [通用测试包 ZIP](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/AnziSend-1.18.3-build131-macos-universal-unsigned.zip) | 支持 Apple 芯片和 Intel 架构。未进行 Developer ID 签名和 Apple 公证，尚未在 Mac 实机验证，系统可能阻止打开。 |
| iOS / iPadOS | 暂无原生安装包 | 可尝试从浏览器使用网页版。 |

下载后可校验文件的 SHA‑256。Windows、Android 和 Linux 使用 [SHA256SUMS.txt](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/SHA256SUMS.txt)，macOS 使用 [SHA256-macOS-build131.txt](https://github.com/wangzebin1716-alt/AnziSend/releases/download/v1.18.3-build131/SHA256-macOS-build131.txt)。

## 常见问题

**连着不同的 Wi‑Fi，也能在没有互联网时传吗？**  
可以，只要两台设备在同一个可互访的内网中。比如企业的办公 Wi‑Fi 与有线网络互通，或校园的两个接入点允许设备互访。若两台设备分属独立的企业网和校园网，则需走跨网络直连。

**为什么按名字找不到对方？**  
先确认对方已连接身份服务、开启了查找，并提供当前设备的 12 位身份码。网页版和已安装的软件各自有设备身份码。遇到同名设备时，用身份码查找，再核对完整指纹。

## 离线传输盒子（设计中）

计划把 USB 接入、Wi‑Fi 热点和本地传输页面集成到一个设备里。原型拟采用电脑通过 USB 接入、手机连接盒子 Wi‑Fi 的方式，由盒子建立局域网。在没有外网的地方，手机可以通过浏览器打开盒子里的传输页。按机型验证接入方式和传输表现后，再确定正式支持范围。

## 反馈

在 AnziSend 软件中打开「反馈建议」即可提交问题或改进建议，提交成功后会看到回执。反馈连接问题时，可以附上双方的软件版本、操作系统、网络类型，以及卡在查找、建立连接还是发送文件。
