---
title: 自动加密某些 Office 365 电子邮件
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509681"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="09b5c-102">自动加密某些 Office 365 电子邮件</span><span class="sxs-lookup"><span data-stu-id="09b5c-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="09b5c-103">您可以自动加密用户发送给特定外部人员或组织的邮件。</span><span class="sxs-lookup"><span data-stu-id="09b5c-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="09b5c-104">为此，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="09b5c-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="09b5c-105">从 [Exchange 管理中心](https://outlook.office365.com/ecp/)， **选择邮件流>规则**。</span><span class="sxs-lookup"><span data-stu-id="09b5c-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="09b5c-106">单击 **"新建 (+)** 图标，然后单击"将 Office **365** 邮件加密和权限保护应用于邮件"。</span><span class="sxs-lookup"><span data-stu-id="09b5c-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="09b5c-107">在 **"名称**"中，输入规则的名称，例如 *加密* 发送到 DrToniRamos@gmail.com。</span><span class="sxs-lookup"><span data-stu-id="09b5c-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="09b5c-108">在 **"如果应用此规则**"中，选择> **收件人是此人**。</span><span class="sxs-lookup"><span data-stu-id="09b5c-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="09b5c-109">在 **"选择成员**"窗口中，选择要应用加密规则的人的姓名，然后单击"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="09b5c-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="09b5c-110">添加完用户后，单击"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="09b5c-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="09b5c-111">在"**执行以下操作"字段旁边**，单击"**选择一个"。**</span><span class="sxs-lookup"><span data-stu-id="09b5c-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="09b5c-112">在 **RMS 模板** 下拉菜单中，**选择"加密**"，然后单击"**确定"。**</span><span class="sxs-lookup"><span data-stu-id="09b5c-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="09b5c-113"> (如果看不到此选项，这意味着你的计划不包括自动加密。</span><span class="sxs-lookup"><span data-stu-id="09b5c-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="09b5c-114">但你可以添加它！) </span><span class="sxs-lookup"><span data-stu-id="09b5c-114">But you can add it!)</span></span>
9. <span data-ttu-id="09b5c-115">从 (可选选择列表中选择任何可选选项，许多可选选择都可以通过默认设置进行选择，以简化) 。</span><span class="sxs-lookup"><span data-stu-id="09b5c-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="09b5c-116">单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="09b5c-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="09b5c-117">稍后始终可以返回并编辑此规则。</span><span class="sxs-lookup"><span data-stu-id="09b5c-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="09b5c-118">有关创建加密规则的信息，请参阅"定义邮件[流规则以加密 Office 365 中的电子邮件"。](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="09b5c-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

