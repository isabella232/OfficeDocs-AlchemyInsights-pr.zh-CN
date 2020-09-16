---
title: 多个对象的电子邮件地址与标识相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724605"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="e7da1-102">多个对象的电子邮件地址与标识相同</span><span class="sxs-lookup"><span data-stu-id="e7da1-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="e7da1-103">**多个对象**</span><span class="sxs-lookup"><span data-stu-id="e7da1-103">**Multiple objects**</span></span>

<span data-ttu-id="e7da1-104">发生此错误的常见原因之一是，如果有多个对象的电子邮件地址与标识相同，则无法正确路由 Outlook Web Access 请求。</span><span class="sxs-lookup"><span data-stu-id="e7da1-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="e7da1-105">若要查找这些对象，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="e7da1-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="e7da1-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="e7da1-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="e7da1-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="e7da1-107">· Get-User <email address></span></span>

<span data-ttu-id="e7da1-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="e7da1-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="e7da1-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="e7da1-109">· Get-Contact <email address></span></span>

<span data-ttu-id="e7da1-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="e7da1-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="e7da1-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="e7da1-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="e7da1-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="e7da1-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="e7da1-113">若要解决该问题，请删除具有相同电子邮件标识的多个对象，并确保有一个对象具有特定电子邮件标识，并且其收件人类型为 UserMailbox。</span><span class="sxs-lookup"><span data-stu-id="e7da1-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="e7da1-114">**相同地址用于企业和使用者邮箱**</span><span class="sxs-lookup"><span data-stu-id="e7da1-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="e7da1-115">另一种原因是将相同地址用于企业和使用者邮箱。</span><span class="sxs-lookup"><span data-stu-id="e7da1-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="e7da1-116">在这种情况下，用户必须更改其主要的使用者别名，直至 Cafe 支持此方案。</span><span class="sxs-lookup"><span data-stu-id="e7da1-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="e7da1-117">这是一个永久性错误，没有干预就不会消失。</span><span class="sxs-lookup"><span data-stu-id="e7da1-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="e7da1-118">有关详细信息，请参阅[更改 Microsoft 帐户的电子邮件地址或电话号码](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)。</span><span class="sxs-lookup"><span data-stu-id="e7da1-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>