---
title: 如何启用无缝 SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: d203c1256785a99426503a5386935d78f8966a8b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384671"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="40a8d-102">如何启用无缝 SSO</span><span class="sxs-lookup"><span data-stu-id="40a8d-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="40a8d-103">通过[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)启用无缝 SSO。</span><span class="sxs-lookup"><span data-stu-id="40a8d-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="40a8d-104">如果要执行 Azure AD Connect 的全新安装, 请选择 "[自定义安装路径](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)"。</span><span class="sxs-lookup"><span data-stu-id="40a8d-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="40a8d-105">在 "**用户登录**" 页上, 选择 "**启用单一登录"** 选项。</span><span class="sxs-lookup"><span data-stu-id="40a8d-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="40a8d-106">若要验证是否正确启用了无缝 SSO, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="40a8d-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="40a8d-107">以全局管理员身份登录到[Azure Active Directory 管理中心](https://aad.portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="40a8d-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="40a8d-108">在左窗格中选择 " **Azure Active Directory** "。</span><span class="sxs-lookup"><span data-stu-id="40a8d-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="40a8d-109">验证是否**启用了**无缝单一登录。</span><span class="sxs-lookup"><span data-stu-id="40a8d-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="40a8d-110">若要了解详细信息, 请参阅[Azure Active Directory 无缝单一登录: 快速入门](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。</span><span class="sxs-lookup"><span data-stu-id="40a8d-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  