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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571778"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="e77b7-102">适用于 Microsoft Edge 的高级身份验证概念</span><span class="sxs-lookup"><span data-stu-id="e77b7-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="e77b7-103">以下是适用于 Microsoft Edge 的高级身份验证概念：</span><span class="sxs-lookup"><span data-stu-id="e77b7-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="e77b7-104">**主动身份验证**</span><span class="sxs-lookup"><span data-stu-id="e77b7-104">**Proactive Authentication**</span></span>

<span data-ttu-id="e77b7-105">启用 [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 策略时，microsoft Edge 将尝试通过 microsoft 服务主动对登录用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e77b7-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="e77b7-106">在固定的时间间隔内，它将使用联机服务来检查包含配置主动身份验证的已更新清单。</span><span class="sxs-lookup"><span data-stu-id="e77b7-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="e77b7-107">好处：主动身份验证允许对关键服务（如 Office "新建" 选项卡页）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e77b7-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="e77b7-108">此外，如果将 Bing 用作搜索引擎，则主动身份验证可提高地址栏的性能，并可帮助生成针对您的业务需求而个性化的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="e77b7-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="e77b7-109">**用于 NTLM 身份验证的 Windows Hello CredUI**</span><span class="sxs-lookup"><span data-stu-id="e77b7-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="e77b7-110">如果在网站尝试通过 NTLM 或协商机制登录用户时，单一登录 (SSO) 不可用，则此功能将允许用户与网站共享 OS 凭据，并通过使用 Windows Hello 凭据 UI 来满足身份验证质询。</span><span class="sxs-lookup"><span data-stu-id="e77b7-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="e77b7-111">此登录流仅在 Windows 10 中显示，并且仅适用于在 NTLM 或协商质询期间未获取 SSO 的用户。</span><span class="sxs-lookup"><span data-stu-id="e77b7-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="e77b7-112">**使用保存的密码自动登录**</span><span class="sxs-lookup"><span data-stu-id="e77b7-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="e77b7-113">在 Microsoft Edge 中保存密码的用户可以启用对其保存凭据的网站的自动登录。</span><span class="sxs-lookup"><span data-stu-id="e77b7-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="e77b7-114">用户可在 edge://settings/passwords 中打开或关闭此功能，您可以在 [密码管理器](https://go.microsoft.com/fwlink/?linkid=2134622) 策略中对其进行配置。</span><span class="sxs-lookup"><span data-stu-id="e77b7-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
