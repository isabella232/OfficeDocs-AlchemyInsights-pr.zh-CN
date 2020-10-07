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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366418"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e2a7c-102">监视对 Exchange 的条件访问</span><span class="sxs-lookup"><span data-stu-id="e2a7c-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e2a7c-103">如果用户不符合组织的访问要求，则以条件访问为目标的用户将收到通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e2a7c-104">若要解决此问题，我们建议采用以下一个或多个解决方案：</span><span class="sxs-lookup"><span data-stu-id="e2a7c-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="e2a7c-105">如果要注册设备，请建议用户转到公司门户应用程序，并验证它是否出现在公司门户中。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e2a7c-106">如果不是，则用户应注册该设备。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="e2a7c-107">在 Azure 门户中，转到 Intune > 设备合规性。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e2a7c-108">在 "监视器单击" "设备符合性" 下。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="e2a7c-109">查看设备合规性报告，以验证用户的设备是否已标记为合规。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="e2a7c-110">在 Azure 门户中，转到 Intune > 设备合规性。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e2a7c-111">在 "管理" 下，单击 "策略"。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-111">Under Manage, click Policies.</span></span> <span data-ttu-id="e2a7c-112">在合规性策略列表中，验证是否已将配置文件分配给您的用户设备。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e2a7c-113">如果未分配任何配置文件，则 Intune 将无法确认设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="e2a7c-114">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="e2a7c-115">在 Azure 门户中，转到**Intune**  >  **条件访问**  >  **策略**。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="e2a7c-116">从列表中选择一个策略。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="e2a7c-117">单击 "用户和组"。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-117">Click Users and groups.</span></span>
4. <span data-ttu-id="e2a7c-118">若要面向某人的特定策略，请将其添加到包含列表中。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="e2a7c-119">若要确保从策略中忽略某个人，请将其添加到 "排除" 列表中。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="e2a7c-120">帮助链接：</span><span class="sxs-lookup"><span data-stu-id="e2a7c-120">Helpful links:</span></span>

[<span data-ttu-id="e2a7c-121">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="e2a7c-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="e2a7c-122">对 CA 进行故障排除</span><span class="sxs-lookup"><span data-stu-id="e2a7c-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e2a7c-123">故障排除策略</span><span class="sxs-lookup"><span data-stu-id="e2a7c-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="e2a7c-124">监控 Intune 设备合规性</span><span class="sxs-lookup"><span data-stu-id="e2a7c-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="e2a7c-125">注意：这些步骤仅有助于对 Azure Active Directory 功能条件访问进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e2a7c-126">此外，还可以通过 Exchange 策略隔离阻止其电子邮件访问的设备。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e2a7c-127">可在 [此处](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)找到有关 Exchange 设备管理的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e2a7c-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
