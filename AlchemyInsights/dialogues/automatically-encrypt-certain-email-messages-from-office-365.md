---
title: 自动加密 Office 365 中的某些电子邮件
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509683"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="c5ea8-102">自动加密 Office 365 中的某些电子邮件</span><span class="sxs-lookup"><span data-stu-id="c5ea8-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="c5ea8-103">从 [Exchange 管理中心](https://outlook.office365.com/ecp/)， **选择邮件流>规则**。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c5ea8-104">单击 **"新建 (+)** 图标，然后单击"将 Office **365** 邮件加密和权限保护应用于邮件"。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c5ea8-105">在 **"名称**"中，输入规则的名称，如 *加密所有邮件*。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="c5ea8-106">在 **"如果应用此规则"中**，选择 **"应用于所有邮件"。**</span><span class="sxs-lookup"><span data-stu-id="c5ea8-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="c5ea8-107">在"**执行以下操作"字段旁边**，单击"**选择一个"。**</span><span class="sxs-lookup"><span data-stu-id="c5ea8-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="c5ea8-108">在 **RMS 模板** 下拉菜单中，**选择"加密**"，然后单击"**确定"。**</span><span class="sxs-lookup"><span data-stu-id="c5ea8-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c5ea8-109"> (如果看不到此选项，这意味着你的计划不包括自动加密。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c5ea8-110">但你可以添加它！) </span><span class="sxs-lookup"><span data-stu-id="c5ea8-110">But you can add it!)</span></span>
7. <span data-ttu-id="c5ea8-111">选中 **"使用严重性级别审核此规则"** 复选框，然后选择所需的级别。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="c5ea8-112">如果你的公司有合同义务发送所有加密的电子邮件，建议将级别设置为 **"高"。**</span><span class="sxs-lookup"><span data-stu-id="c5ea8-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="c5ea8-113">在 **"为此规则选择模型"下**，单击"**强制"。**</span><span class="sxs-lookup"><span data-stu-id="c5ea8-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="c5ea8-114">从 (可选选择列表中选择任何可选选择选项，其中很多选项都可以使用默认设置，以简化) 。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c5ea8-115">单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c5ea8-116">稍后你始终可以返回并编辑此规则。</span><span class="sxs-lookup"><span data-stu-id="c5ea8-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c5ea8-117">有关创建加密规则的信息，请参阅["定义邮件流规则以加密 Office 365 中的电子邮件](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)"</span><span class="sxs-lookup"><span data-stu-id="c5ea8-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

