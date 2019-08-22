---
title: 如何禁用外部组
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540891"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="cbdbc-102">如何禁用外部组</span><span class="sxs-lookup"><span data-stu-id="cbdbc-102">How to disable External Groups</span></span>

<span data-ttu-id="cbdbc-103">Yammer 外部邮件应用 Exchange 传输规则 (Etr), 这是一组用于防止公司信息被共享的主动控制。</span><span class="sxs-lookup"><span data-stu-id="cbdbc-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="cbdbc-104">为了限制用户创建外部组, 您需要配置 Exchange 传输规则 (ETR), 然后将 Yammer 配置为使用 Exchange 传输规则来阻止外部邮件。</span><span class="sxs-lookup"><span data-stu-id="cbdbc-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="cbdbc-105">在 Exchange Online 管理中心中创建规则后, 请按照以下步骤设置 ETR 以在 Yammer 中应用:</span><span class="sxs-lookup"><span data-stu-id="cbdbc-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="cbdbc-106">以经验证的管理员身份登录到 Yammer, 并在**Yammer 管理中心**中, 转到 "C **Content And \> security security Settings"。**</span><span class="sxs-lookup"><span data-stu-id="cbdbc-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="cbdbc-107">在 "**外部邮件**" 下, 选择 "在**Yammer 中强制实施 Exchange Online exchange 传输规则 (etr)"。**</span><span class="sxs-lookup"><span data-stu-id="cbdbc-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="cbdbc-108">选择“保存”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="cbdbc-108">Choose **Save**.</span></span>

<span data-ttu-id="cbdbc-109">有关详细信息, 请参阅在[具有 Exchange 传输规则的 Yammer 网络中控制外部消息](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="cbdbc-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  