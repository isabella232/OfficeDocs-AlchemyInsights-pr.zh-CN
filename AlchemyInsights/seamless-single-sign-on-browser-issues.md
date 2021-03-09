---
title: SSO 的无缝单一登录 (解决) 问题
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
- "9004357"
- "9377"
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530815"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="23173-102">SSO 的无缝单一登录 (解决) 问题</span><span class="sxs-lookup"><span data-stu-id="23173-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="23173-103">大多数用户都能够通过以下步骤解决其无缝 SSO 浏览器问题：</span><span class="sxs-lookup"><span data-stu-id="23173-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="23173-104">确保浏览器是最新的。</span><span class="sxs-lookup"><span data-stu-id="23173-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="23173-105">从浏览器中删除 Cookie 以删除无效的 SSO 会话，然后再次尝试登录。</span><span class="sxs-lookup"><span data-stu-id="23173-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="23173-106">尝试使用其他浏览器登录。</span><span class="sxs-lookup"><span data-stu-id="23173-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="23173-107">**已知的浏览器问题**</span><span class="sxs-lookup"><span data-stu-id="23173-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="23173-108">Firefox 上的无缝 SSO 在专用浏览模式下不起作用。</span><span class="sxs-lookup"><span data-stu-id="23173-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="23173-109">当启用增强保护模式时，Internet Explorer SSO 无法正常使用。</span><span class="sxs-lookup"><span data-stu-id="23173-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="23173-110">无缝 SSO 在 Microsoft Edge 上的专用浏览模式下 (旧版) 。</span><span class="sxs-lookup"><span data-stu-id="23173-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="23173-111">无缝 SSO 在 iOS 和 Android 上的移动浏览器上不起作用。</span><span class="sxs-lookup"><span data-stu-id="23173-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="23173-112">无缝 SSO 支持基于 Chromium 的下一版本的 Microsoft Edge，并且它按设计在 InPrivate 和来宾模式下工作。</span><span class="sxs-lookup"><span data-stu-id="23173-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="23173-113">**公告**</span><span class="sxs-lookup"><span data-stu-id="23173-113">**Advisory**</span></span>

<span data-ttu-id="23173-114">若要提出功能请求或询问有关无缝 SSO 的技术问题，请参阅 [Microsoft 问答&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span><span class="sxs-lookup"><span data-stu-id="23173-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
