---
title: 自动加密发送到特定域的 Office 365 电子邮件
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735633"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="d7242-102">自动加密发送到特定域的 Office 365 电子邮件</span><span class="sxs-lookup"><span data-stu-id="d7242-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="d7242-103">从 [Exchange 管理中心，](https://outlook.office365.com/ecp/)选择"**邮件流>规则"。**</span><span class="sxs-lookup"><span data-stu-id="d7242-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="d7242-104">单击" **新建 (+) "** 图标，然后单击"将 Office **365** 邮件加密和权限保护应用于邮件"。</span><span class="sxs-lookup"><span data-stu-id="d7242-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="d7242-105">在 **"** 名称"中，输入规则的名称，例如"加密发送到 *contoso.com"。*</span><span class="sxs-lookup"><span data-stu-id="d7242-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="d7242-106">在 **"在应用此规则时"** 中 **，选择">域为 "。**</span><span class="sxs-lookup"><span data-stu-id="d7242-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="d7242-107">输入域的名称，**例如contoso.com。**</span><span class="sxs-lookup"><span data-stu-id="d7242-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="d7242-108">单击"**添加 (+) "** 图标，然后单击"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="d7242-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="d7242-109">在"执行以下操作 **"字段旁边**，单击"选择 **一个"。**</span><span class="sxs-lookup"><span data-stu-id="d7242-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="d7242-110">在 **RMS 模板下拉菜单中**，选择"加密 **"，** 然后单击"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="d7242-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="d7242-111"> (如果未看到此选项，则意味着你的计划不包括自动加密。</span><span class="sxs-lookup"><span data-stu-id="d7242-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="d7242-112">但你可以添加它！) </span><span class="sxs-lookup"><span data-stu-id="d7242-112">But you can add it!)</span></span>
9. <span data-ttu-id="d7242-113">从此时 (可选选择列表中选择任何可选选项，其中很多选项都可以使用默认设置，以简化) 。</span><span class="sxs-lookup"><span data-stu-id="d7242-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="d7242-114">单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="d7242-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d7242-115">稍后始终可以返回并编辑此规则。</span><span class="sxs-lookup"><span data-stu-id="d7242-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="d7242-116">有关创建加密规则的信息，请参阅在[Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)中定义用于加密电子邮件的邮件流规则</span><span class="sxs-lookup"><span data-stu-id="d7242-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>