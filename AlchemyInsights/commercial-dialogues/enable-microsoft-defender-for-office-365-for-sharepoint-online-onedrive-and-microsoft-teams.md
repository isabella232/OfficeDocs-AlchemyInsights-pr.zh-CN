---
title: 为 保险箱 Online、SharePoint 和 OneDrive 启用Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332369"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>为 保险箱 Online、SharePoint 和 OneDrive 启用Microsoft Teams

1. 使用全局管理员或安全管理员凭据，在 中打开 Microsoft 365 Defender 门户，然后转到"策略"部分中的"策略"&规则"威胁策略保险箱 <https://security.microsoft.com>  \>  \> **附件**" 

   若要直接转到"附件 **保险箱，** 请使用 <https://security.microsoft.com/safeattachmentv2> 。

2. 在 **"保险箱"页上**，单击"**全局设置"。**
3. On the flyout that appears， select **Turn on Microsoft Defender for Office 365 for SharePoint， OneDrive， and Microsoft Teams**， and then select **Save**.

    **提示**：执行以下步骤可增强对保险箱、SharePoint和OneDrive附件Microsoft Teams：
    - 若要阻止用户下载恶意文件，请使用 `$true` SharePoint Online PowerShell 中 **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** cmdlet 的 *DisallowInfectedFileDownload* 参数的值。 有关详细信息，请参阅使用[SharePoint Online PowerShell 阻止用户下载恶意文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)。
    - [为检测到的文件创建警报策略](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

有关详细信息，请参阅 保险箱[Attachments for Office 365 for SharePoint， OneDrive， and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041)。
