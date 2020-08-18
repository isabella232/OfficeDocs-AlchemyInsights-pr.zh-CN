---
title: 更改适用于 Office 的更新通道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786843"
---
# <a name="change-update-channels-for-office-apps"></a>更改适用于 Office 的更新通道

对于全新的 Office 安装，请使用 Office 软件下载设置选择所需的更新通道，然后安装（或重新安装） Office 应用。 有关更多信息，请参阅[在 Office 365 中管理软件下载设置](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)。 

**注意** 使用 Office 软件下载设置选择的更新通道适用于使用 O365 门户执行新安装的所有用户。 有关详细信息，请参阅[在电脑或 Mac 上下载并安装或重新安装 Microsoft 365 或 Office 2019](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)。   

对于现有 Office 安装，请使用 Office 部署工具（ODT）切换到其他更新通道：  

1. 从 [Microsoft下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载最新版本的 Office 部署工具（setup.exe）。
2. 标识要切换到的频道名称。 有关详细信息，请参阅 [Office 部署工具的配置选项](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)。
3. 创建一个配置XML文件，指定适当的通道名称，例如 update.xml。  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. 从提升的命令提示符处，切换到 setup.exe 所在的文件夹位置并运行以下命令：  
    a. setup.exe /configure update.xml
5. 启动 Office 应用程序（例如 Excel ），然后选择“**文件**” > “**帐户**”。 在“产品信息”部分中，选择“**更新选项**” > “**立即更新**”。

有关更多信息，请参阅[如何切换现有 Office 应用的更新通道](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)。 

若要切换所选用户组的更新通道或使用配置管理器（SCCM），请使用 GPO 配置更新通道设置。 有关详细信息，请参阅 [Microsoft 365 应用版的更新频道概述](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)。 有关详细信息，请参阅[如何管理适用于 IT专业人员的 Office 365 ProPlus 通道](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813)和[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 应用版更新](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)。