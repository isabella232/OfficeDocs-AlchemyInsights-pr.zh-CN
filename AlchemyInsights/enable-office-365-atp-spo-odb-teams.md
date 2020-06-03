---
title: 为 SharePoint、OneDrive 和 Microsoft 团队启用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506908"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 SharePoint Online、OneDrive 和 Microsoft 团队启用 Office 365 高级威胁防护

1. 转到 https://protection.office.com 并登录。
2. 选择**威胁管理**  >  **策略**  >  **安全附件**。
3. 选择 "**启用 SharePoint、OneDrive 和 Microsoft 团队的 ATP**"，然后单击 "**保存**"。
4. 适合作为全局管理员或 SharePoint Online 管理员，运行[set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet，并将**DisallowInfectedFileDownload**参数设置为*true*。
5. 适合为检测到的文件[设置警报](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)。

> [!NOTE]
> ATP 将在 SharePoint Online、OneDrive 或 Microsoft 团队中扫描每个单个文件。 文件通过使用共享和来宾活动事件的进程进行异步扫描，同时还通过智能启发和威胁信号来识别恶意文件。 请参阅[适用于 SharePoint、OneDrive 和 Microsoft 团队的 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。