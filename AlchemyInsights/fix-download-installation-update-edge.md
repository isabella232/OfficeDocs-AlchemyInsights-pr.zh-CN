---
title: 修复 Microsoft Edge 的下载、安装和更新问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9128"
- "9004429"
ms.openlocfilehash: 3db5fc4f2be0bbf845dec15b53f1299653f97ed75e12b04e8041de5982f5a74a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945910"
---
# <a name="fix-problems-with-the-download-installation-and-update-of-microsoft-edge"></a>修复 Microsoft Edge 的下载、安装和更新问题

在尝试进行任何修复之前，请验证计算机操作系统是否与 Microsoft Edge 兼容，后者支持 Windows 10、8、8.1、7 32 位 (x86) 和 64 位 (x64) 以及 macOS 10.12 Sierra 及更高版本。若要修复 Microsoft Edge 下载、安装和更新方面的问题，请按照以下说明进行操作：

1. 检查网络和 VPN：
    - 检查网络连接。
    - 如果出现 403 错误，则表明 VPN 可能会阻止下载。 断开与 VPN 的连接，然后再次尝试下载Microsoft Edge。
1. 将 officeapps.live.com 添加到浏览器受信任的网站列表。
    例如，如果使用 Internet Explorer 下载Microsoft Edge：
    1. 选择 **工具** > **Internet 选项**。
    2. 在"**安全**"选项卡中，选择 **受信任的站点** > **站点**。
    3. 在"**将此网站添加到区域**"下，键入<https://officeapps.live.com>，选择"**添加**"，然后选择"**关闭**"。
1. 在 Windows 计算机上重新安装 Microsoft Edge， 无需卸载 Microsoft Edge 即可重新安装。 此外，重新安装不会影响历史记录、Cookie 和设置。

    在 Mac 上，必须先卸载 Microsoft Edge，然后才能重新安装。 此外，还必须还原历史记录、Cookie 和设置。

    卸载 Mac 上的 Microsoft Edge：
    1. 打开“查找工具”。
    2. 在 **应用程序** 文件夹中，选择 **Microsoft Edge**。
    3. 选择 **文件** > **移动到回收站**。

    若要在 Windows 或 Mac 计算机上重新安装Microsoft Edge：
    1. 打开任何正常工作的浏览器。
    2. 转到 Microsoft Edge 下载网站，下载并重新安装浏览器。
1. 重启计算机：重新启动计算机，然后尝试重新安装Microsoft Edge。

