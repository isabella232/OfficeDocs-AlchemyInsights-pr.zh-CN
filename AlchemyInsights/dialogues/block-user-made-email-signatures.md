---
title: 阻止用户创建的电子邮件签名
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232696"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="aad4b-102">阻止用户创建的电子邮件签名</span><span class="sxs-lookup"><span data-stu-id="aad4b-102">Block user-made email signatures</span></span>

<span data-ttu-id="aad4b-103">以下解决方案仅适用于在 Web 上的 Outlook 中创建的电子邮件签名。</span><span class="sxs-lookup"><span data-stu-id="aad4b-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="aad4b-104">只有在具有本地部署时，才能阻止 Outlook 应用中的Exchange Server。</span><span class="sxs-lookup"><span data-stu-id="aad4b-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="aad4b-105">在管理中心中，选择 **"管理中心**  >  **Exchange"。**</span><span class="sxs-lookup"><span data-stu-id="aad4b-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="aad4b-106">单击 **策略**  >  **Outlook Web App权限**。</span><span class="sxs-lookup"><span data-stu-id="aad4b-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="aad4b-107">选择策略，然后单击铅笔图标进行编辑。</span><span class="sxs-lookup"><span data-stu-id="aad4b-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="aad4b-108">单击 **功能**  >  **更多选项**。</span><span class="sxs-lookup"><span data-stu-id="aad4b-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="aad4b-109">在 **"用户体验"** 下，清除"**电子邮件签名**"复选框，然后单击"保存 **"。**</span><span class="sxs-lookup"><span data-stu-id="aad4b-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="aad4b-110">**重要提示：** 如果在清除此复选框之前添加了签名，用户仍可以使用它。</span><span class="sxs-lookup"><span data-stu-id="aad4b-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="aad4b-111">要求他们删除它。</span><span class="sxs-lookup"><span data-stu-id="aad4b-111">Ask them to remove it.</span></span>
