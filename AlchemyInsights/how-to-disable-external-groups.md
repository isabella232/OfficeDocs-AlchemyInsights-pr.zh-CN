---
title: 如何禁用外部组
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720758"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2b663-102">如何禁用外部组</span><span class="sxs-lookup"><span data-stu-id="2b663-102">How to disable External Groups</span></span>

<span data-ttu-id="2b663-103">Yammer 外部邮件应用 Exchange 传输规则（Etr），这是一组用于防止公司信息被共享的主动控制。</span><span class="sxs-lookup"><span data-stu-id="2b663-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2b663-104">为了限制用户创建外部组，您需要配置 Exchange 传输规则（ETR），然后将 Yammer 配置为使用 Exchange 传输规则来阻止外部邮件。</span><span class="sxs-lookup"><span data-stu-id="2b663-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="2b663-105">在 Exchange Online 管理中心中创建规则后，请按照以下步骤设置 ETR 以在 Yammer 中应用：</span><span class="sxs-lookup"><span data-stu-id="2b663-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2b663-106">以经验证的管理员身份登录到 Yammer，并在**Yammer 管理中心**中，转到 "C **Content And \> security security Settings"。**</span><span class="sxs-lookup"><span data-stu-id="2b663-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="2b663-107">在 "**外部邮件**" 下，选择 "在**Yammer 中强制实施 Exchange Online exchange 传输规则（etr）"。**</span><span class="sxs-lookup"><span data-stu-id="2b663-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="2b663-108">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="2b663-108">Choose **Save**.</span></span>

<span data-ttu-id="2b663-109">有关详细信息，请参阅在[Yammer 网络中禁用外部消息](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)。</span><span class="sxs-lookup"><span data-stu-id="2b663-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  