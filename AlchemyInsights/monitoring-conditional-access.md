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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708664"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="52911-102">监视 Exchange 的条件访问</span><span class="sxs-lookup"><span data-stu-id="52911-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="52911-103">如果条件访问的目标用户不符合组织的访问要求，他们将收到一封通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="52911-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="52911-104">若要解决，我们建议使用以下一个或多个解决方案：</span><span class="sxs-lookup"><span data-stu-id="52911-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="52911-105">如果认为设备已注册，建议用户转到公司门户应用并验证它是否显示在公司门户中。</span><span class="sxs-lookup"><span data-stu-id="52911-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="52911-106">如果没有，则用户应注册设备。</span><span class="sxs-lookup"><span data-stu-id="52911-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="52911-107">在 Azure 门户中，转到 Intune >设备合规性。</span><span class="sxs-lookup"><span data-stu-id="52911-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="52911-108">在"监视器"下单击"设备合规性"。</span><span class="sxs-lookup"><span data-stu-id="52911-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="52911-109">查看设备合规性报告，验证用户设备是否标记为合规。</span><span class="sxs-lookup"><span data-stu-id="52911-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="52911-110">在 Azure 门户中，转到 Intune >设备合规性。</span><span class="sxs-lookup"><span data-stu-id="52911-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="52911-111">在"管理"下，单击"策略"。</span><span class="sxs-lookup"><span data-stu-id="52911-111">Under Manage, click Policies.</span></span> <span data-ttu-id="52911-112">在合规性策略列表中，验证配置文件是否分配给用户设备。</span><span class="sxs-lookup"><span data-stu-id="52911-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="52911-113">如果未分配任何配置文件，则 Intune 将无法确认设备的合规性状态。</span><span class="sxs-lookup"><span data-stu-id="52911-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="52911-114">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="52911-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="52911-115">在 Azure 门户中，转到 **Intune**  >  **条件访问**  >  **策略**。</span><span class="sxs-lookup"><span data-stu-id="52911-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="52911-116">从列表中选择策略。</span><span class="sxs-lookup"><span data-stu-id="52911-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="52911-117">单击"用户和组"。</span><span class="sxs-lookup"><span data-stu-id="52911-117">Click Users and groups.</span></span>
4. <span data-ttu-id="52911-118">若要将特定策略面向某人，请将其添加到"包含"列表中。</span><span class="sxs-lookup"><span data-stu-id="52911-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="52911-119">若要确保策略中省略某人，请将其添加到排除列表中。</span><span class="sxs-lookup"><span data-stu-id="52911-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="52911-120">有用链接：</span><span class="sxs-lookup"><span data-stu-id="52911-120">Helpful links:</span></span>

[<span data-ttu-id="52911-121">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="52911-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="52911-122">CA 疑难解答</span><span class="sxs-lookup"><span data-stu-id="52911-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="52911-123">疑难解答策略</span><span class="sxs-lookup"><span data-stu-id="52911-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="52911-124">监视 Intune 设备合规性</span><span class="sxs-lookup"><span data-stu-id="52911-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="52911-125">注意：这些步骤仅有助于对 Azure Active Directory 功能条件访问进行疑难解答。</span><span class="sxs-lookup"><span data-stu-id="52911-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="52911-126">也可以隔离使用 Exchange 策略阻止其电子邮件访问的设备。</span><span class="sxs-lookup"><span data-stu-id="52911-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="52911-127">有关 Exchange 设备管理详细信息，请参阅[此处 https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) ] (。</span><span class="sxs-lookup"><span data-stu-id="52911-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
