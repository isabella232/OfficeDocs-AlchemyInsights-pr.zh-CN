---
title: 监视条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702893"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e596e-102">监视对 Exchange 的条件访问</span><span class="sxs-lookup"><span data-stu-id="e596e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e596e-103">如果用户不符合组织的访问要求，则以条件访问为目标的用户将收到通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e596e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e596e-104">若要解决此问题，我们建议采用以下一个或多个解决方案：</span><span class="sxs-lookup"><span data-stu-id="e596e-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e596e-105">如果要注册设备，请建议用户转到公司门户应用程序，并验证它是否出现在公司门户中。</span><span class="sxs-lookup"><span data-stu-id="e596e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e596e-106">如果不是，则用户应注册该设备。</span><span class="sxs-lookup"><span data-stu-id="e596e-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e596e-107">在 Azure 门户中，转到 **Intune \> 设备符合性**。</span><span class="sxs-lookup"><span data-stu-id="e596e-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e596e-108">在 " **监视器** 单击" " **设备符合性**" 下。</span><span class="sxs-lookup"><span data-stu-id="e596e-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e596e-109">查看设备合规性报告，以验证用户的设备是否已标记为合规。</span><span class="sxs-lookup"><span data-stu-id="e596e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e596e-110">在 Azure 门户中，转到 **Intune \> 设备符合性**。</span><span class="sxs-lookup"><span data-stu-id="e596e-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e596e-111">在 " **管理**" 下，单击 " **策略**"。</span><span class="sxs-lookup"><span data-stu-id="e596e-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e596e-112">在合规性策略列表中，验证是否已将配置文件分配给您的用户设备。</span><span class="sxs-lookup"><span data-stu-id="e596e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e596e-113">如果未分配任何配置文件，则 Intune 将无法确认设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="e596e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e596e-114">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="e596e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e596e-115">在 Azure 门户中，转到 **Intune \> 条件访问 \> 策略**</span><span class="sxs-lookup"><span data-stu-id="e596e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e596e-116">从列表中选择策略</span><span class="sxs-lookup"><span data-stu-id="e596e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e596e-117">单击 "**用户和组**"</span><span class="sxs-lookup"><span data-stu-id="e596e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e596e-118">若要面向某人的特定策略，请将其添加到 **包含** 列表中。</span><span class="sxs-lookup"><span data-stu-id="e596e-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e596e-119">若要确保从策略中忽略某个人，请将其添加到 " **排除** " 列表中。</span><span class="sxs-lookup"><span data-stu-id="e596e-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e596e-120">阅读详细信息： [如何监视条件访问设备](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e596e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

