---
title: Microsoft Defender for Office 365 反网络钓鱼策略示例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552276"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="3be19-102">Microsoft Defender for Office 365 反网络钓鱼策略示例</span><span class="sxs-lookup"><span data-stu-id="3be19-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="3be19-103">这些设置启用名为"域"和 *"CEO"的策略*。</span><span class="sxs-lookup"><span data-stu-id="3be19-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="3be19-104">此策略提供用户和域保护，防止模拟，然后将该策略应用于域中用户接收的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3be19-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="3be19-105">首先，添加以下信息以创建策略：</span><span class="sxs-lookup"><span data-stu-id="3be19-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="3be19-106">**名称**：域和 CEO **说明**：确保 CEO 和您的域未被模拟。</span><span class="sxs-lookup"><span data-stu-id="3be19-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="3be19-107">**应用于：** 选择 **收件人域为**。</span><span class="sxs-lookup"><span data-stu-id="3be19-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="3be19-108">在 **任一项下**， **选择"选择**"，然后选择域。</span><span class="sxs-lookup"><span data-stu-id="3be19-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="3be19-109">选择“+ 添加”。</span><span class="sxs-lookup"><span data-stu-id="3be19-109">Select **+ Add**.</span></span> <span data-ttu-id="3be19-110">选中列表中域名称旁边的复选框 (例如，contoso.com) ，然后选择"**添加"。** </span><span class="sxs-lookup"><span data-stu-id="3be19-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="3be19-111">选择“**完成**”。</span><span class="sxs-lookup"><span data-stu-id="3be19-111">Select **Done**.</span></span>
- <span data-ttu-id="3be19-112">创建策略后，可以使用以下选项微调策略：</span><span class="sxs-lookup"><span data-stu-id="3be19-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="3be19-113">**添加要保护的用户：** 对于此示例，至少添加 CEO 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3be19-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="3be19-114">**添加要保护的域**：添加包含 CEO 办公室的组织域。</span><span class="sxs-lookup"><span data-stu-id="3be19-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="3be19-115">**选择操作**：如果 **电子邮件** 是由模拟用户发送的，请选择"将邮件重定向到另一个电子邮件地址"，然后输入安全管理员的电子邮件地址 (例如，securityadmin@contoso.com) 。 </span><span class="sxs-lookup"><span data-stu-id="3be19-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="3be19-116">For **If email is sent by an impersonated domain，** select Quarantine the **message.**</span><span class="sxs-lookup"><span data-stu-id="3be19-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="3be19-117">**邮箱智能**：默认情况下，当您创建新的防钓鱼策略时，将选择此选项。</span><span class="sxs-lookup"><span data-stu-id="3be19-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="3be19-118">最好将此设置保留为“打开”。</span><span class="sxs-lookup"><span data-stu-id="3be19-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="3be19-119">**添加受信任的发件人和域：** 对于此示例，不要定义任何替代。</span><span class="sxs-lookup"><span data-stu-id="3be19-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="3be19-120">查看设置后，选择"创建此策略" **或** " **保存**"（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="3be19-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="3be19-121">若要了解更多信息，请参阅 [Microsoft 365 中的防钓鱼策略](https://go.microsoft.com/fwlink/?linkid=2092235)。</span><span class="sxs-lookup"><span data-stu-id="3be19-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
