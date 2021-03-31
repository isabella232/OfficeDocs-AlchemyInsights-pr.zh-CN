---
title: 126 在 OWA 中找不到邮箱错误？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426652"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="5b921-102">在 Web 上的 Outlook 中收到未找到邮箱的错误？</span><span class="sxs-lookup"><span data-stu-id="5b921-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="5b921-103">如果使用的是 Outlook 网页版，但因错误而找不到邮箱，则用于连接到 Outlook 网页版的帐户没有 Exchange Online 许可证，因此没有邮箱与该帐户关联。</span><span class="sxs-lookup"><span data-stu-id="5b921-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="5b921-104">管理员可通过执行以下步骤将许可证分配给你的帐户：</span><span class="sxs-lookup"><span data-stu-id="5b921-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="5b921-105">打开[Microsoft 365 管理](https://portal.office.com/adminportal/home#/homepage)中心，转到"用户"部分下的"活动用户"，然后选择看到错误的用户。</span><span class="sxs-lookup"><span data-stu-id="5b921-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="5b921-106">在打开的用户页面中，转到"许可证和应用"部分，选择相应的 **"** 位置"值，并分配包含 Exchange Online (的许可证，以查看其详细信息) 。</span><span class="sxs-lookup"><span data-stu-id="5b921-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="5b921-107">完成后，单击“**保存更改**”。</span><span class="sxs-lookup"><span data-stu-id="5b921-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="5b921-108">在某些情况下，如果许可证已分配给用户帐户，则删除和重新分配许可证有助于解决问题，并正确在系统中进行预配：</span><span class="sxs-lookup"><span data-stu-id="5b921-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="5b921-109">检查你的 M365 Exchange Online 订阅 (（如果有）是否) 订阅当前且尚未过期。</span><span class="sxs-lookup"><span data-stu-id="5b921-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="5b921-110">一旦确保你的订阅未过期并且向用户帐户分配了有效的许可证，设置许可证可能需要 24 小时，因此你可能必须等待问题解决。</span><span class="sxs-lookup"><span data-stu-id="5b921-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="5b921-111">有关详细信息，请参阅分配 [和管理许可证](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)。</span><span class="sxs-lookup"><span data-stu-id="5b921-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>