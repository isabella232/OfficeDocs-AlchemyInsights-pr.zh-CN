---
title: 为Office 365、SharePoint和OneDrive启用 ATP Microsoft Teams
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332149"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 Office 365 Online、SharePoint 和 OneDrive 启用 Microsoft Defender Microsoft Teams

1. 转到 https://protection.office.com 并登录。
2. 选择 **"威胁管理**  >  **策略**  >  **保险箱附件"。**
3. 选择 **打开 Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams，****然后单击保存。**
4.  (建议) 全局管理员或 SharePoint Online 管理员，运行 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet，将 **DisallowInfectedFileDownload** 参数设置为 *true。*
5.  (推荐) [设置检测到的文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 的警报。

**注意**：Microsoft Defender for Office 365不会扫描 SharePoint Online、OneDrive 或 Microsoft Teams。 通过使用共享和来宾活动事件以及智能启发和威胁信号识别恶意文件的过程，以异步方式扫描文件。 请参阅[Microsoft Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams。](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
