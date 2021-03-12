---
title: 为混合环境配置邮件加密
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735529"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="1268a-102">为混合环境配置邮件加密</span><span class="sxs-lookup"><span data-stu-id="1268a-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="1268a-103">对于混合 Exchange 环境，只有当电子邮件通过 Exchange Online 路由时，本地用户可以使用 Office 邮件加密 (OME) 发送加密电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1268a-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="1268a-104">若要使用 OME 加密电子邮件，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="1268a-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="1268a-105">使用 ["混合配置"](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) 向导设置混合环境。</span><span class="sxs-lookup"><span data-stu-id="1268a-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="1268a-106">设置加密不需要任何特殊步骤。</span><span class="sxs-lookup"><span data-stu-id="1268a-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="1268a-107">[像通常一样设置邮件流](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) 规则进行加密。</span><span class="sxs-lookup"><span data-stu-id="1268a-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


