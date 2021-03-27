---
title: 适用于 Microsoft Edge 的高级身份验证概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398542"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="d3877-102">适用于 Microsoft Edge 的高级身份验证概念</span><span class="sxs-lookup"><span data-stu-id="d3877-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="d3877-103">以下是适用于 Microsoft Edge 的高级身份验证概念：</span><span class="sxs-lookup"><span data-stu-id="d3877-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="d3877-104">**主动身份验证**</span><span class="sxs-lookup"><span data-stu-id="d3877-104">**Proactive Authentication**</span></span>

<span data-ttu-id="d3877-105">启用 [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 策略后，Microsoft Edge 将尝试通过 Microsoft 服务主动验证登录用户的身份。</span><span class="sxs-lookup"><span data-stu-id="d3877-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="d3877-106">它定期使用联机服务检查更新的清单，其中包含管理主动身份验证的配置。</span><span class="sxs-lookup"><span data-stu-id="d3877-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="d3877-107">优点：主动身份验证支持对关键服务（如 Office 新选项卡页）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d3877-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="d3877-108">此外，如果将必应用作搜索引擎，则主动身份验证可改进地址栏的性能，并帮助生成个性化的搜索结果以满足业务需求。</span><span class="sxs-lookup"><span data-stu-id="d3877-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="d3877-109">**用于 NTLM 身份验证的 Windows Hello CredUI**</span><span class="sxs-lookup"><span data-stu-id="d3877-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="d3877-110">如果单一登录 (SSO) 在网站尝试通过 NTLM 或协商机制登录用户时不可用，则此功能将允许用户与网站共享操作系统凭据，并通过使用 Windows Hello Cred UI 满足身份验证质询。</span><span class="sxs-lookup"><span data-stu-id="d3877-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="d3877-111">此登录流程将仅在 Windows 10 中显示，并且仅适用于在 NTLM 或协商质询期间未获取 SSO 的用户。</span><span class="sxs-lookup"><span data-stu-id="d3877-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="d3877-112">**使用保存的密码自动登录**</span><span class="sxs-lookup"><span data-stu-id="d3877-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="d3877-113">在 Microsoft Edge 中保存密码的用户可以启用自动登录到已保存凭据的网站。</span><span class="sxs-lookup"><span data-stu-id="d3877-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="d3877-114">用户可以在密码管理器中打开或 edge://settings/passwords 此功能，并且您可以在密码管理器 [策略中对其进行](https://go.microsoft.com/fwlink/?linkid=2134622) 配置。</span><span class="sxs-lookup"><span data-stu-id="d3877-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
