---
title: 设置电子邮件转发
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787127"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="ceb3c-102">检查邮箱的电子邮件转发设置</span><span class="sxs-lookup"><span data-stu-id="ceb3c-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="ceb3c-103">首先，必须启用租户级别的电子邮件转发。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="ceb3c-104">如果您在邮箱上设置了电子邮件转发，但它未运行 (则看到错误 **"550 5.7.520** 访问被拒绝，你的组织不允许外部转发") 请参阅在 [Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)中控制自动外部电子邮件转发。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="ceb3c-105">验证邮箱中的电子邮件转发设置非常简单！</span><span class="sxs-lookup"><span data-stu-id="ceb3c-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="ceb3c-106">只需执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="ceb3c-107">如果这是用户邮箱，请转到"用户 \> **""活动** 用户"，然后选择要转发其邮箱的用户。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="ceb3c-108">在"**邮件"** 选项卡上，选择 **"管理电子邮件转发"。**</span><span class="sxs-lookup"><span data-stu-id="ceb3c-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="ceb3c-109">如果这是共享邮箱，请转到"组""共享邮箱"，然后选择要 \> 转发的共享邮箱。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="ceb3c-110">选择 **"** 编辑"进行电子邮件转发。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="ceb3c-111">有关详细信息，请参阅在 [Microsoft 365 中配置电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="ceb3c-112">若要向用户发送说明，以便他们可以在其自己的邮箱上设置电子邮件转发，请将其指向"将电子邮件从[Microsoft 365 转发到另一个电子邮件帐户"。](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)</span><span class="sxs-lookup"><span data-stu-id="ceb3c-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="ceb3c-113">请注意，只能转发到一个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="ceb3c-114">如果需要设置转发给一组人员，请创建通讯组列表 (组 **) ，** 将用户添加到该组，然后配置转发到该组。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="ceb3c-115">你是否有员工离开？</span><span class="sxs-lookup"><span data-stu-id="ceb3c-115">Do you have an employee leaving?</span></span> <span data-ttu-id="ceb3c-116">有关建议步骤，请参阅从 [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) 中删除以前的员工。</span><span class="sxs-lookup"><span data-stu-id="ceb3c-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>