---
title: 多个对象的电子邮件地址与标识相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431341"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="4f23c-102">多个对象的电子邮件地址与标识相同</span><span class="sxs-lookup"><span data-stu-id="4f23c-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="4f23c-103">**多个对象**</span><span class="sxs-lookup"><span data-stu-id="4f23c-103">**Multiple objects**</span></span>

<span data-ttu-id="4f23c-104">发生此错误的常见原因之一是，如果有多个对象的电子邮件地址与标识相同，则无法正确路由 Outlook Web Access 请求。</span><span class="sxs-lookup"><span data-stu-id="4f23c-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="4f23c-105">若要查找这些对象，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="4f23c-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="4f23c-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="4f23c-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="4f23c-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="4f23c-107">· Get-User <email address></span></span>

<span data-ttu-id="4f23c-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="4f23c-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="4f23c-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="4f23c-109">· Get-Contact <email address></span></span>

<span data-ttu-id="4f23c-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="4f23c-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="4f23c-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="4f23c-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="4f23c-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="4f23c-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="4f23c-113">若要解决该问题，请删除具有相同电子邮件标识的多个对象，并确保有一个对象具有特定电子邮件标识，并且其收件人类型为 UserMailbox。</span><span class="sxs-lookup"><span data-stu-id="4f23c-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="4f23c-114">**相同地址用于企业和使用者邮箱**</span><span class="sxs-lookup"><span data-stu-id="4f23c-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="4f23c-115">另一种原因是将相同地址用于企业和使用者邮箱。</span><span class="sxs-lookup"><span data-stu-id="4f23c-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="4f23c-116">在这种情况下，用户必须更改其主要的使用者别名，直至 Cafe 支持此方案。</span><span class="sxs-lookup"><span data-stu-id="4f23c-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="4f23c-117">这是一个永久性错误，没有干预就不会消失。</span><span class="sxs-lookup"><span data-stu-id="4f23c-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="4f23c-118">有关详细信息，请参阅[更改 Microsoft 帐户的电子邮件地址或电话号码](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)。</span><span class="sxs-lookup"><span data-stu-id="4f23c-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>