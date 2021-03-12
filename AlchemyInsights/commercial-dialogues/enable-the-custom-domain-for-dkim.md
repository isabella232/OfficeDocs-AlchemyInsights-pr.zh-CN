---
title: 为 DKIM 启用自定义域
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735626"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="4a338-102">为 DKIM 启用自定义域</span><span class="sxs-lookup"><span data-stu-id="4a338-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="4a338-103">为自定义域创建 CNAME 记录后，需要启用域。</span><span class="sxs-lookup"><span data-stu-id="4a338-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="4a338-104">若要启用域，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="4a338-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="4a338-105">导航到 [Exchange 管理中心](https://outlook.office365.com/ecp/)。</span><span class="sxs-lookup"><span data-stu-id="4a338-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="4a338-106">在左窗格中，选择 **"dkim >保护"。**</span><span class="sxs-lookup"><span data-stu-id="4a338-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="4a338-107">选择域，然后在"使用 **DKIM** 签名为此域签名邮件"下，单击"启用 **"。**</span><span class="sxs-lookup"><span data-stu-id="4a338-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="4a338-108">对每个域重复此步骤。</span><span class="sxs-lookup"><span data-stu-id="4a338-108">Repeat this step for each domain.</span></span>

