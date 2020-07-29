---
title: 控制 Office 应用的自动更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431360"
---
# <a name="control-automatic-updates-for-office-apps"></a>控制 Office 应用的自动更新

默认情况下，Office 应用的更新会自动下载并在后台应用，无需任何用户干预。 但是，管理员可以使用 Office Update 设置控制更新的应用方式。 更新设置允许管理员启用或禁用自动更新、显示或隐藏 Office 中的“**立即更新**”按钮、设置更新截止日期等。 有关详细信息，请参阅：

- [配置 Office 的更新设置](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office 的自动更新未启用](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [定义 Office 安装后的更新方式](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

若要查看应用于客户端计算机的现有更新设置，请按照以下步骤进行操作：

1. 转到“**开始**” > “**运行**” > “**regedit**”，打开注册表编辑器。
2. 切换到以下位置并查看 Office Update 设置：  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**注意** 如果设置了OfficeMgmtCOM 注册表项，则可能会在“**Office**” > “**帐户**” > “**Office Updates**”中看到“更新由系统管理员管理”消息。 有关详细信息，请参阅[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 应用版更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)。  