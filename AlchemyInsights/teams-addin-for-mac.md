---
title: Mac 版 Teams 外接程序
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617044"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="d1803-102">Mac 版 Teams 外接程序</span><span class="sxs-lookup"><span data-stu-id="d1803-102">Teams add-in for Mac</span></span>

<span data-ttu-id="d1803-103">若要对 Mac 操作系统用户缺失 Teams 外接程序进行故障排除，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="d1803-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="d1803-104">**步骤 1：** 如果你有混合 Exchange 本地（需要 2016 CU3 或更高版本），请使用 Test-HMA.ps1 工具确认已正确配置混合新式验证。</span><span class="sxs-lookup"><span data-stu-id="d1803-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="d1803-105">有关详细信息，请参阅[验证用于 Outlook for iOS 和 Outlook for Android 的混合新式验证设置](https://aka.ms/AA980zq)。</span><span class="sxs-lookup"><span data-stu-id="d1803-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="d1803-106">**注意** 使用 UPN 地址格式（例如 [username@contoso.com](mailto:username@contoso.com)），而不是域\用户名。</span><span class="sxs-lookup"><span data-stu-id="d1803-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="d1803-107">即使对于具有 Exchange Online 邮箱的用户，也要这样做。</span><span class="sxs-lookup"><span data-stu-id="d1803-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="d1803-108">**步骤 2：** 让用户在 Outlook for Mac 中转到“**工具**” > “**帐户...**”，然后查找并选择帐户。</span><span class="sxs-lookup"><span data-stu-id="d1803-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="d1803-109">确认列出的用户名采用 UPN 格式（例如 [username@contoso.com](mailto:username@contoso.com)）。</span><span class="sxs-lookup"><span data-stu-id="d1803-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="d1803-110">**步骤 3：** 确认用户是许可的 Microsoft Teams 用户。</span><span class="sxs-lookup"><span data-stu-id="d1803-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="d1803-111">用户必须使用 Office 365 for Mac 订阅、产品版本 16.24 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d1803-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>