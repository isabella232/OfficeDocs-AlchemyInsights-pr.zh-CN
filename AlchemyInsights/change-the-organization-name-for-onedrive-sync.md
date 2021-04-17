---
title: 更改 OneDrive 同步客户端的组织名称
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003077"
- "5850"
ms.openlocfilehash: ca545ba51e39209f3302acdee1c24048515e2c1b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818314"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="b2689-102">更改 OneDrive 同步客户端的组织名称</span><span class="sxs-lookup"><span data-stu-id="b2689-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="b2689-103">OneDrive 使用由租户管理员设置的组织名称。</span><span class="sxs-lookup"><span data-stu-id="b2689-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="b2689-104">你可以[更改组织的地址、技术联系人和其他信息](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)。</span><span class="sxs-lookup"><span data-stu-id="b2689-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="b2689-105">对租户执行此更改后，在用户取消链接并重新链接其 OneDrive 帐户之前，OneDrive 同步客户端将不会反映新名称。</span><span class="sxs-lookup"><span data-stu-id="b2689-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="b2689-106">若要取消链接帐户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b2689-106">To unlink the account:</span></span>

1. <span data-ttu-id="b2689-107">选择任务栏最右侧的蓝色 OneDrive 云图标，然后选择 **“更多”>“设置”>“帐户”**。</span><span class="sxs-lookup"><span data-stu-id="b2689-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="b2689-108">找到要取消链接的帐户，然后依次选择“**取消链接此电脑**”和“**取消链接帐户**”。</span><span class="sxs-lookup"><span data-stu-id="b2689-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="b2689-109">若要重新链接帐户，请从“设置”的“**帐户**”选项卡中选择“**添加帐户**”，然后重新登录到 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="b2689-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>