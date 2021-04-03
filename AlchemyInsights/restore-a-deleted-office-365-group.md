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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505672"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="1040d-102">还原已删除的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="1040d-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="1040d-103">可以在删除后 30 天内还原已删除的 Microsoft 365 组或 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="1040d-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="1040d-104">若要登录到 Microsoft 365 管理中心并列出已删除的组和团队，请转到 [Microsoft 365 管理中心](https://aka.ms/RestoreDeletedGroup)。</span><span class="sxs-lookup"><span data-stu-id="1040d-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="1040d-105">**注意：** 使用分配给租户管理员或组管理员角色的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="1040d-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="1040d-106">选择要还原的已删除的 Microsoft 365 组/Teams，然后单击"**还原组"。**</span><span class="sxs-lookup"><span data-stu-id="1040d-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="1040d-107">如果由于 SMTP 地址冲突而无法还原组，请使用以下命令查找导致冲突的对象并删除 SMTP 地址：</span><span class="sxs-lookup"><span data-stu-id="1040d-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="1040d-108">**注意：** 在某些情况下，可能需要 24 小时才能还原组及其所有数据。</span><span class="sxs-lookup"><span data-stu-id="1040d-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="1040d-109">有关详细信息，或了解如何使用 PowerShell 还原组，请参阅还原 [已删除的 Microsoft 365 组](https://go.microsoft.com/fwlink/?linkid=867802)。</span><span class="sxs-lookup"><span data-stu-id="1040d-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>