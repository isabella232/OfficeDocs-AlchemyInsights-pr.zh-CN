---
title: 如何启用无缝 SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780517"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="8fbc8-102">如何启用无缝 SSO</span><span class="sxs-lookup"><span data-stu-id="8fbc8-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="8fbc8-103">通过 [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)启用无缝 SSO。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="8fbc8-104">如果要执行 Azure AD Connect 的全新安装，请选择 " [自定义安装路径](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)"。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="8fbc8-105">在 " **用户登录** " 页上，选择 " **启用单一登录"** 选项。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="8fbc8-106">若要验证是否正确启用了无缝 SSO，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="8fbc8-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="8fbc8-107">以全局管理员身份登录到 [Azure Active Directory 管理中心](https://aad.portal.azure.com) 。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="8fbc8-108">在左窗格中选择 " **Azure Active Directory** "。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="8fbc8-109">验证是否 **启用了**无缝单一登录。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="8fbc8-110">若要了解详细信息，请参阅 [Azure Active Directory 无缝单一登录：快速入门](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。</span><span class="sxs-lookup"><span data-stu-id="8fbc8-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  