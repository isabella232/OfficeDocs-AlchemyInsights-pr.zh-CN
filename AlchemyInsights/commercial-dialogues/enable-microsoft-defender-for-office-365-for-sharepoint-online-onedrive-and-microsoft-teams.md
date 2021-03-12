---
title: 为 SharePoint Online、OneDrive 和 Microsoft Teams 启用 Microsoft Defender for Office 365
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735513"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 SharePoint Online、OneDrive 和 Microsoft Teams 启用 Microsoft Defender for Office 365

1. 使用全局管理员或安全管理员凭据，登录到 [Office 365 安全与合规中心](https://protection.office.com/)。
2. 在 **左窗格中选择**"威胁管理"，然后选择"**策略**  >  [安全附件"。](https://protection.office.com/safeattachment)
3. 选择 **"打开适用于 SharePoint、OneDrive 和 Microsoft Teams 的 Microsoft Defender for Office 365"，** 然后选择"保存 **"。**
    > [!TIP]
    >
    > - 作为全局管理员或 SharePoint Online 管理员，运行以下 PowerShell cmdlet，将 **DisallowInfectedFileDownload** 参数设置为 [true：Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301) 
    > - [为检测到的文件设置警报](https://go.microsoft.com/fwlink/?linkid=2092110)

有关详细信息，请参阅[Microsoft Defender for Office 365 for SharePoint、 OneDrive 和 Microsoft Teams。](https://go.microsoft.com/fwlink/?linkid=2092041)
