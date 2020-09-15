---
title: 为 SharePoint、OneDrive 和 Microsoft 团队启用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709897"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 SharePoint Online、OneDrive 和 Microsoft 团队启用 Office 365 高级威胁防护

1. 转到 https://protection.office.com 并登录。
2. 选择**威胁管理**  >  **策略**  >  **安全附件**。
3. 选择 " **启用 SharePoint、OneDrive 和 Microsoft 团队的 ATP**"，然后单击 " **保存**"。
4.  (推荐) 为全局管理员或 SharePoint Online 管理员，请运行 [set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet，并将 **DisallowInfectedFileDownload** 参数设置为 *true*。
5.  (建议的) 为检测到的文件 [设置通知](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 。

> [!NOTE]
> ATP 将在 SharePoint Online、OneDrive 或 Microsoft 团队中扫描每个单个文件。 文件通过使用共享和来宾活动事件的进程进行异步扫描，同时还通过智能启发和威胁信号来识别恶意文件。 请参阅 [适用于 SharePoint、OneDrive 和 Microsoft 团队的 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。