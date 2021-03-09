---
title: 修复 Microsoft Defender for Office 365 的常见问题
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552275"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="9e5e2-102">修复 Microsoft Defender for Office 365 的常见问题</span><span class="sxs-lookup"><span data-stu-id="9e5e2-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="9e5e2-103">下面是 Microsoft Defender for Office 365 常见问题的一些解决方案：</span><span class="sxs-lookup"><span data-stu-id="9e5e2-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="9e5e2-104">**邮件延迟：** 如果遇到邮件传递延迟的问题，您需要在安全附件策略内使用动态传递选项。 </span><span class="sxs-lookup"><span data-stu-id="9e5e2-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="9e5e2-105">若要了解更多信息，请参阅["安全附件策略中的动态传递"。](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="9e5e2-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="9e5e2-106">**报告误报或负结果：** 使用此链接将邮件报告给 [Microsoft：Microsoft Defender 响应门户](https://go.microsoft.com/fwlink/?linkid=2092835)。</span><span class="sxs-lookup"><span data-stu-id="9e5e2-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="9e5e2-107">**启用安全链接保护：**</span><span class="sxs-lookup"><span data-stu-id="9e5e2-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="9e5e2-108">登录到 Office [365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="9e5e2-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="9e5e2-109">转到 **"威胁管理**  >  **策略**  >  **安全链接"。**</span><span class="sxs-lookup"><span data-stu-id="9e5e2-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="9e5e2-110">在 **"应用于特定收件人的策略"下**，打开配置的策略。</span><span class="sxs-lookup"><span data-stu-id="9e5e2-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="9e5e2-111">在 **"设置**"**下，选择"将安全链接应用于在组织内部发送的邮件"。**</span><span class="sxs-lookup"><span data-stu-id="9e5e2-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
