---
title: 通知 AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897540"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="b2b12-102">通知 AAD Connect</span><span class="sxs-lookup"><span data-stu-id="b2b12-102">Notification AAD Connect</span></span>

- <span data-ttu-id="b2b12-103">确保你有权执行此操作。</span><span class="sxs-lookup"><span data-stu-id="b2b12-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="b2b12-104">默认情况下，全局管理员具有访问权限。</span><span class="sxs-lookup"><span data-stu-id="b2b12-104">Global Admins have access by default.</span></span> <span data-ttu-id="b2b12-105">此外，您可以使用基于 [角色的访问控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 将注册权限委派给参与者。</span><span class="sxs-lookup"><span data-stu-id="b2b12-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="b2b12-106">确保所需的终结点已启用，并且不会因防火墙而受阻。</span><span class="sxs-lookup"><span data-stu-id="b2b12-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="b2b12-107">有关详细信息，请参阅 [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。</span><span class="sxs-lookup"><span data-stu-id="b2b12-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="b2b12-108">由于出站通信受到网络层 SSL 检查，注册可能会失败。</span><span class="sxs-lookup"><span data-stu-id="b2b12-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="b2b12-109">确保你已验证 Azure AD Connect Health 的通知设置并查看你的设置。</span><span class="sxs-lookup"><span data-stu-id="b2b12-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="b2b12-110">若要了解如何配置 Azure AD Connect Health 通知的通知设置，请参阅 [本指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)。</span><span class="sxs-lookup"><span data-stu-id="b2b12-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="b2b12-111">若要了解有关 AAD Connect Health 同步报告以及如何下载它，请参阅对象 [级同步报告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。</span><span class="sxs-lookup"><span data-stu-id="b2b12-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="b2b12-112">若要解决 AAD Connect 运行状况警报问题，请按照 [AAD Connect Health 数据](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 新鲜度警报疑难解答指南操作，有关常见问题，请参阅 [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。</span><span class="sxs-lookup"><span data-stu-id="b2b12-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
