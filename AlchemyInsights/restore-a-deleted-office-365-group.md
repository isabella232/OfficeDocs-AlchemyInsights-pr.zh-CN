---
title: 还原已删除的 Microsoft 365 组
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597433"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="2e595-102">还原已删除的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="2e595-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="2e595-103">可以在删除后 30 天内还原已删除的 Microsoft 365 组或 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="2e595-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="2e595-104">转到 [Microsoft 365 管理](https://aka.ms/RestoreDeletedGroup) 中心登录并列出已删除的组和团队。</span><span class="sxs-lookup"><span data-stu-id="2e595-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="2e595-105">**注意：** 使用分配给租户管理员或组管理员角色的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="2e595-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="2e595-106">选择要还原的已删除的 Microsoft 365 组/Teams，然后单击"**还原组"。**</span><span class="sxs-lookup"><span data-stu-id="2e595-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="2e595-107">如果由于 SMTP 地址冲突而无法还原组，请使用以下命令查找导致冲突的对象并删除 SMTP 地址：</span><span class="sxs-lookup"><span data-stu-id="2e595-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="2e595-108">**注意：** 在某些情况下，可能需要 24 小时才能还原组及其所有数据。</span><span class="sxs-lookup"><span data-stu-id="2e595-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="2e595-109">有关详细信息，或了解如何使用 PowerShell 还原组，请参阅还原 [已删除的 Microsoft 365 组](https://go.microsoft.com/fwlink/?linkid=867802)。</span><span class="sxs-lookup"><span data-stu-id="2e595-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>