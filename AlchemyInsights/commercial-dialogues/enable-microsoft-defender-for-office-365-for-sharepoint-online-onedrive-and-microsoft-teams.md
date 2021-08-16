---
title: 为 Office 365 Online、SharePoint 和 OneDrive 启用 Microsoft Defender Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058856"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 Office 365 Online、SharePoint 和 OneDrive 启用 Microsoft Defender Microsoft Teams

1. 使用全局管理员或安全管理员凭据，登录到Office 365[安全与合规中心。](https://protection.office.com/)
2. 在 **左窗格中选择**"威胁管理"，然后选择"**策略保险箱**  >  [附件"。](https://protection.office.com/safeattachment)
3. 选择 **打开 Microsoft Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams，****然后选择保存。**
    > [!TIP]
    >
    > - 作为全局管理员或 SharePoint Online 管理员，运行以下 PowerShell cmdlet，将 **DisallowInfectedFileDownload** 参数设置为 [true：Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301) 
    > - [为检测到的文件设置警报](https://go.microsoft.com/fwlink/?linkid=2092110)

有关详细信息，请参阅[Microsoft Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams。](https://go.microsoft.com/fwlink/?linkid=2092041)
