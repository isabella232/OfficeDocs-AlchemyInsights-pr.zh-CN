---
title: 监视 Intune 条件访问
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416983"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="ac783-102">监视 Intune 条件访问</span><span class="sxs-lookup"><span data-stu-id="ac783-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="ac783-103">如果条件访问的目标用户不符合组织的访问要求，他们将收到一封通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ac783-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ac783-104">若要解决，我们建议使用以下一个或多个解决方案：</span><span class="sxs-lookup"><span data-stu-id="ac783-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="ac783-105">如果认为设备已注册，建议用户转到公司门户应用，并验证它是否显示在公司门户中。</span><span class="sxs-lookup"><span data-stu-id="ac783-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ac783-106">如果没有，用户必须注册设备。</span><span class="sxs-lookup"><span data-stu-id="ac783-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="ac783-107">在 Azure 门户中，转到 **Intune**  >  **设备合规性**。</span><span class="sxs-lookup"><span data-stu-id="ac783-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="ac783-108">若要查看设备合规性报告以验证用户设备是否标记为合规，请在 **"** 监视器"下，单击 **"设备合规性"。**</span><span class="sxs-lookup"><span data-stu-id="ac783-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="ac783-109">在 Azure 门户中，转到 **Intune**  >  **设备合规性**。</span><span class="sxs-lookup"><span data-stu-id="ac783-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="ac783-110">在 **"管理"下**，单击 **"策略"。**</span><span class="sxs-lookup"><span data-stu-id="ac783-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="ac783-111">在合规性策略列表中，验证配置文件是否分配给用户设备。</span><span class="sxs-lookup"><span data-stu-id="ac783-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ac783-112">如果未分配任何配置文件，则 Intune 将无法确认设备的合规性状态。</span><span class="sxs-lookup"><span data-stu-id="ac783-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="ac783-113">编辑用户的条件访问分配。</span><span class="sxs-lookup"><span data-stu-id="ac783-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="ac783-114">在 Azure 门户中，导航到 **Intune**  >  **条件访问**  >  **策略**，从列表中选择策略，然后单击"**用户和组"。**</span><span class="sxs-lookup"><span data-stu-id="ac783-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="ac783-115">若要将特定策略面向某人，请将其添加到 **"包含"列表中**。</span><span class="sxs-lookup"><span data-stu-id="ac783-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="ac783-116">若要确保从策略中省略某人，请将其添加到排除 **列表中**。</span><span class="sxs-lookup"><span data-stu-id="ac783-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="ac783-117">**有用链接：**</span><span class="sxs-lookup"><span data-stu-id="ac783-117">**Helpful links:**</span></span>

- [<span data-ttu-id="ac783-118">设备合规性概述</span><span class="sxs-lookup"><span data-stu-id="ac783-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="ac783-119">CA 疑难解答</span><span class="sxs-lookup"><span data-stu-id="ac783-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="ac783-120">疑难解答策略</span><span class="sxs-lookup"><span data-stu-id="ac783-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="ac783-121">监视 Intune 设备合规性</span><span class="sxs-lookup"><span data-stu-id="ac783-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="ac783-122">这些步骤仅有助于对 Azure Active Directory 功能条件访问进行疑难解答。</span><span class="sxs-lookup"><span data-stu-id="ac783-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="ac783-123">也可以隔离使用 Exchange 策略阻止其电子邮件访问的设备。</span><span class="sxs-lookup"><span data-stu-id="ac783-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="ac783-124">有关 Exchange 设备管理详细信息，请参阅 [**此处**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))。</span><span class="sxs-lookup"><span data-stu-id="ac783-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
