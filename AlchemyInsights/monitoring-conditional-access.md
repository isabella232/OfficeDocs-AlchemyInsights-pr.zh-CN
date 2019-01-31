---
title: 监控条件的访问
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656557"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="cf65b-102">监控条件的访问</span><span class="sxs-lookup"><span data-stu-id="cf65b-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="cf65b-p101">目标具有条件的访问权限的用户将收到通知电子邮件，如果他们不能满足您组织的访问要求。若要解决，我们建议一个或多个以下解决方案：</span><span class="sxs-lookup"><span data-stu-id="cf65b-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="cf65b-p102">如果设备则假定为注册，告知用户转到的公司门户应用程序并验证是否显示在公司门户。如果没有，用户应注册设备。</span><span class="sxs-lookup"><span data-stu-id="cf65b-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="cf65b-p103">在 Azure 门户中，转到**Intune\>设备合规性**。在**监视**下单击**设备合规性**。查看您的设备合规性报告，以验证用户的设备已标记为兼容。</span><span class="sxs-lookup"><span data-stu-id="cf65b-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="cf65b-p104">在 Azure 门户中，转到**Intune\>设备合规性**。在**管理**下单击**策略**。在合规性策略列表中，验证该配置文件分配给用户的设备。如果没有分配配置，然后 Intune 将不能以确认设备的合规性状态。</span><span class="sxs-lookup"><span data-stu-id="cf65b-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="cf65b-114">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="cf65b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="cf65b-115">在 Azure 门户中，转到**Intune\>条件访问\>策略**</span><span class="sxs-lookup"><span data-stu-id="cf65b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="cf65b-116">从列表中选择一个策略</span><span class="sxs-lookup"><span data-stu-id="cf65b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="cf65b-117">单击**用户和组**</span><span class="sxs-lookup"><span data-stu-id="cf65b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="cf65b-p105">针对特定的策略某人时，将其添加到**包括**列表。若要确保人员省略从策略，请将其添加到**排除**列表中。</span><span class="sxs-lookup"><span data-stu-id="cf65b-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="cf65b-120">阅读其他信息：[如何监视条件访问设备](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="cf65b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

