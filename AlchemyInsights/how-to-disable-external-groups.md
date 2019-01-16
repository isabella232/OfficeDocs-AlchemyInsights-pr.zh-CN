---
title: 如何禁用外部组
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277108"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="abddc-102">如何禁用外部组</span><span class="sxs-lookup"><span data-stu-id="abddc-102">How to disable External Groups</span></span>

<span data-ttu-id="abddc-p101">Yammer 外部消息适用 Exchange 传输规则 (ETRs)，一套主动控件，以防止公司信息共享。若要创建外部组限制用户，您需要配置 Exchange 传输规则 (ETR)，然后配置为使用 Exchange 传输规则以阻止外部消息的 Yammer。</span><span class="sxs-lookup"><span data-stu-id="abddc-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="abddc-105">一旦您已在 Exchange Online 管理中心创建规则，请按照下列步骤，设置 ETR 应用 Yammer 中：</span><span class="sxs-lookup"><span data-stu-id="abddc-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="abddc-106">登录到 Yammer 为已验证的管理员，并且**Yammer 管理中心**中，转到 C **ontent 和安全\>安全设置。**</span><span class="sxs-lookup"><span data-stu-id="abddc-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="abddc-107">在**外部消息**下选择**强制在 Yammer 中的 Exchange Online Exchange 传输规则 (ETRs)。**</span><span class="sxs-lookup"><span data-stu-id="abddc-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="abddc-108">选择" **保存**"。</span><span class="sxs-lookup"><span data-stu-id="abddc-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="abddc-109">有关详细信息，请参阅[外部消息与 Exchange 传输规则的 Yammer 网络中的控件](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="abddc-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

