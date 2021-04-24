---
title: Exchange 管理中心中的保留策略无法工作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952218"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8ec19-102">Exchange 管理中心中的保留策略</span><span class="sxs-lookup"><span data-stu-id="8ec19-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8ec19-103">如果您希望我们针对下面提到的设置运行自动检查，请选择此页面顶部的"后退"按钮"<"，然后输入与保留策略有问题的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8ec19-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="8ec19-104">如果 Exchange 管理中心中的保留策略无法应用于邮箱或项目未移动到存档邮箱，请检查以下各项：</span><span class="sxs-lookup"><span data-stu-id="8ec19-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="8ec19-105">**根本原因：**</span><span class="sxs-lookup"><span data-stu-id="8ec19-105">**Root Causes:**</span></span>

- <span data-ttu-id="8ec19-106">**托管文件夹** 助理尚未处理用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="8ec19-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8ec19-107">托管文件夹助理每七天尝试处理一次基于云的组织内每个邮箱。</span><span class="sxs-lookup"><span data-stu-id="8ec19-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="8ec19-108">**解决方案：** 运行托管文件夹助理。</span><span class="sxs-lookup"><span data-stu-id="8ec19-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="8ec19-109">已在邮箱上 **启用** **RetentionHold。**</span><span class="sxs-lookup"><span data-stu-id="8ec19-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8ec19-110">如果邮箱已置于 RetentionHold 中，则在此期间将不会处理邮箱的保留策略。</span><span class="sxs-lookup"><span data-stu-id="8ec19-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="8ec19-111">**解决方案：** 根据需要检查"保留保留"设置和更新的状态。</span><span class="sxs-lookup"><span data-stu-id="8ec19-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="8ec19-112">有关详细信息，请参阅邮箱 [保留保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="8ec19-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="8ec19-113">**注意：** 如果邮箱小于 10 MB，托管文件夹助理不会自动处理邮箱。</span><span class="sxs-lookup"><span data-stu-id="8ec19-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8ec19-114">有关 Exchange 管理中心中的保留策略详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="8ec19-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="8ec19-115">保留标记和保留策略</span><span class="sxs-lookup"><span data-stu-id="8ec19-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="8ec19-116">[将保留策略应用于邮箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 或 [添加或删除保留标记](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="8ec19-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="8ec19-117">如何识别为邮箱设置的保留类型</span><span class="sxs-lookup"><span data-stu-id="8ec19-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
