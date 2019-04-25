---
title: 监视条件访问
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418459"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="f997b-102">监视条件访问</span><span class="sxs-lookup"><span data-stu-id="f997b-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="f997b-103">如果用户不符合组织的访问要求, 则以条件访问为目标的用户将收到通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f997b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f997b-104">若要解决此问题, 我们建议采用以下一个或多个解决方案:</span><span class="sxs-lookup"><span data-stu-id="f997b-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="f997b-105">如果要注册设备, 请建议用户转到公司门户应用程序, 并验证它是否出现在公司门户中。</span><span class="sxs-lookup"><span data-stu-id="f997b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f997b-106">如果不是, 则用户应注册该设备。</span><span class="sxs-lookup"><span data-stu-id="f997b-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="f997b-107">在 Azure 门户中, 转**到\> Intune 设备符合性**。</span><span class="sxs-lookup"><span data-stu-id="f997b-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f997b-108">在 "**监视器**单击" "**设备符合性**" 下。</span><span class="sxs-lookup"><span data-stu-id="f997b-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="f997b-109">查看设备合规性报告, 以验证用户的设备是否已标记为合规。</span><span class="sxs-lookup"><span data-stu-id="f997b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="f997b-110">在 Azure 门户中, 转**到\> Intune 设备符合性**。</span><span class="sxs-lookup"><span data-stu-id="f997b-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f997b-111">在 "**管理**" 下, 单击 "**策略**"。</span><span class="sxs-lookup"><span data-stu-id="f997b-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="f997b-112">在合规性策略列表中, 验证是否已将配置文件分配给您的用户设备。</span><span class="sxs-lookup"><span data-stu-id="f997b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f997b-113">如果未分配任何配置文件, 则 Intune 将无法确认设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="f997b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="f997b-114">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="f997b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="f997b-115">在 Azure 门户中, 转**到\> Intune 条件\>访问策略**</span><span class="sxs-lookup"><span data-stu-id="f997b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="f997b-116">从列表中选择策略</span><span class="sxs-lookup"><span data-stu-id="f997b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="f997b-117">单击 "**用户和组**"</span><span class="sxs-lookup"><span data-stu-id="f997b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="f997b-118">若要面向某人的特定策略, 请将其添加到**包含**列表中。</span><span class="sxs-lookup"><span data-stu-id="f997b-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="f997b-119">若要确保从策略中忽略某个人, 请将其添加到 "**排除**" 列表中。</span><span class="sxs-lookup"><span data-stu-id="f997b-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="f997b-120">阅读详细信息:[如何监视条件访问设备](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="f997b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

