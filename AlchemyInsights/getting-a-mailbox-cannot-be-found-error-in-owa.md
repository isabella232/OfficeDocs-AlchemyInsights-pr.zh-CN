---
title: 126在 OWA 中找不到获取邮箱的错误？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105229"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="08a0f-102">在 web 上的 Outlook 中获取 "找不到邮箱" 错误？</span><span class="sxs-lookup"><span data-stu-id="08a0f-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="08a0f-103">如果您使用的是 web 上的 Outlook，但**无法找到错误的邮箱**，则用于连接到 web 上的 outlook 的帐户没有 Exchange Online 许可证，因此没有邮箱与该帐户相关联。</span><span class="sxs-lookup"><span data-stu-id="08a0f-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="08a0f-104">您的管理员可以通过执行以下步骤，将许可证分配给您的帐户：</span><span class="sxs-lookup"><span data-stu-id="08a0f-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="08a0f-105">打开[Microsoft 365 管理中心](https://portal.office.com/adminportal/home#/homepage)并转到 "**用户**" 部分下的 "**活动用户**"，然后选择查看错误的用户。</span><span class="sxs-lookup"><span data-stu-id="08a0f-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="08a0f-106">在打开的用户页中，转到 "**许可证和应用**" 部分，选择适当的 "**位置**" 值，然后分配包含 Exchange Online 的许可证（展开许可证以查看其详细信息）。</span><span class="sxs-lookup"><span data-stu-id="08a0f-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="08a0f-107">完成后，单击 "**保存更改**"。</span><span class="sxs-lookup"><span data-stu-id="08a0f-107">When you're finished, click **Save changes**.</span></span>
