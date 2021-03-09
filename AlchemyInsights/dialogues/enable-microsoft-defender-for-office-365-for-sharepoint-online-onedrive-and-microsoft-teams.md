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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552277"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4d5c4-102">为 SharePoint Online、OneDrive 和 Microsoft Teams 启用 Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="4d5c4-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="4d5c4-103">使用全局管理员或安全管理员凭据，登录到 [Office 365 安全与合规中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="4d5c4-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="4d5c4-104">选择 **左窗格中** 的威胁管理，然后选择 **"策略**  >  [安全附件"。](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="4d5c4-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="4d5c4-105">选择 **打开适用于 SharePoint、OneDrive 和 Microsoft Teams 的 Microsoft Defender for Office 365，** 然后选择"**保存"。**</span><span class="sxs-lookup"><span data-stu-id="4d5c4-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="4d5c4-106">作为全局管理员或 SharePoint Online 管理员，运行以下 PowerShell cmdlet，**将 DisallowInfectedFileDownload** 参数设置为 [true：Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301) </span><span class="sxs-lookup"><span data-stu-id="4d5c4-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="4d5c4-107">为检测到的文件设置警报</span><span class="sxs-lookup"><span data-stu-id="4d5c4-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="4d5c4-108">有关详细信息，请参阅[Microsoft Defender for Office 365 for SharePoint、OneDrive 和 Microsoft Teams。](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="4d5c4-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
