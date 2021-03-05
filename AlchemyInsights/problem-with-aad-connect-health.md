---
title: AAD Connect Health 出现问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453288"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="9325c-102">AAD Connect Health 出现问题</span><span class="sxs-lookup"><span data-stu-id="9325c-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="9325c-103">确保您有权执行此操作。</span><span class="sxs-lookup"><span data-stu-id="9325c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="9325c-104">默认情况下，全局管理员具有访问权限。</span><span class="sxs-lookup"><span data-stu-id="9325c-104">Global Admins have access by default.</span></span> <span data-ttu-id="9325c-105">此外，可以使用基于 [角色的访问控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 将注册权限委派给参与者。</span><span class="sxs-lookup"><span data-stu-id="9325c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="9325c-106">确保所需的终结点已启用，并且由于防火墙未阻止。</span><span class="sxs-lookup"><span data-stu-id="9325c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="9325c-107">有关详细信息，请参阅 [要求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。</span><span class="sxs-lookup"><span data-stu-id="9325c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="9325c-108">由于出站通信受到网络层 SSL 检查，注册可能会失败。</span><span class="sxs-lookup"><span data-stu-id="9325c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="9325c-109">确保已验证 Azure AD Connect Health 的通知设置。</span><span class="sxs-lookup"><span data-stu-id="9325c-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="9325c-110">请查看你的设置。</span><span class="sxs-lookup"><span data-stu-id="9325c-110">Please review your setting.</span></span> <span data-ttu-id="9325c-111">本指南 [可帮助](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) 你了解如何配置 Azure AD Connect 运行状况通知的通知设置。</span><span class="sxs-lookup"><span data-stu-id="9325c-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="9325c-112">若要了解有关 AAD Connect Health 同步报告以及如何下载它，请参阅对象 [级同步报告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。</span><span class="sxs-lookup"><span data-stu-id="9325c-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="9325c-113">若要对 AAD Connect Health 警报进行故障排除，请按照 [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 数据新鲜度警报的疑难解答指南操作，有关常见问题，请参阅 [Common AAD Connect Health 安装问题](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。</span><span class="sxs-lookup"><span data-stu-id="9325c-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
