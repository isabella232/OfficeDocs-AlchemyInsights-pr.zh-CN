---
title: VPN 相关问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505179"
---
# <a name="vpn-related-issues"></a>VPN 相关问题

成功实现 MDM 客户端的 VPN 连接取决于已部署的配置文件，此配置文件可正确反映 VPN 基础结构的要求。 有关正在调查的客户端平台的相应设置，请参阅： 

[使用 Intune 添加 VPN 连接的 Windows 10 和 Windows 全息设备设置](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[在 Microsoft Intune 中添加 iOS 和 iPadOS 设备 VPN 设置](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Intune 中配置 VPN 的 Android 设备设置](https://docs.microsoft.com/intune/vpn-settings-android)  
[在 Microsoft Intune 中添加 macOS 设备 VPN 设置](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

如果你的 VPN 配置文件使用基于证书的身份验证，请确保已成功部署链接到 VPN 配置文件的根证书和客户端身份验证证书配置文件。

**常见问题**

**我将 VPN 配置文件部署到设备。 Intune 显示已成功，但设备未连接到VPN。**

成功状态表示 Intune 已按照配置成功部署了配置文件。 但是，这些配置可能不符合您的网络和/或身份验证要求。 查看基础设施和身份验证服务中的日志（在 VPN 服务器和 NPS / Radius 服务器上），以获取有关尝试的连接的更多详细信息。 可能需要与网络基础设施团队或第三方 VPN 供应商合作，以收集和查看日志。

**配置适用于 iOS 的自定义 VPN 时，每应用 VPN 功能不可用。**

当前，Intune 中适用于 iOS 设备的每应用程序 VPN 适用于特定的提供商和合作伙伴列表，配置每应用 VPN 之前，还必须满足证书的先决条件。 有关更多信息，请参阅[在 Intune 中为 iOS / iPadOS 设备设置每个应用程序的虚拟专用网络 (VPN)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)。 

有关 Intune 中所有 VPN 连接类型的详细信息，请参阅[创建 VPN 配置文件以连接到 Intune 中的 VPN 服务器](https://docs.microsoft.com/intune/vpn-settings-configure)。  

**访问配置的域时，iOS 按需 VPN 未触发**

要测试自动 VPN 设置，请设定以下值：

我要执行以下操作：**评估每一连接尝试** 

选择是否连接：**根据需要连接**

用户访问以下域时：**目标** *域名*

如果以上配置不成功，请添加以下元素：

无法访问该 URL 时，强制连接 VPN： **BADURL**