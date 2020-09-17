---
title: 解决 Teams 登录错误 AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687028"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="954a3-102">解决 Teams 登录错误 AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="954a3-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="954a3-103">登录 Microsoft Teams 时，可能会收到以下错误：**抱歉，在 AADSTS9000411 中登录时遇到问题：请求的格式不正确。参数“login_hint”重复。**</span><span class="sxs-lookup"><span data-stu-id="954a3-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="954a3-104">若要解决此问题，请确保你的 Microsoft Teams 客户端已更新。</span><span class="sxs-lookup"><span data-stu-id="954a3-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="954a3-105">有关更新客户端的详细信息，请参阅 [更新 Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="954a3-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="954a3-106">如果由于某种原因无法更新客户端，注销客户端将清除大部分缓存数据。</span><span class="sxs-lookup"><span data-stu-id="954a3-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="954a3-107">但是，如果在注销/登录后仍遇到问题，请退出 Teams 并执行以下操作来清除客户端缓存：</span><span class="sxs-lookup"><span data-stu-id="954a3-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="954a3-108">关闭 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="954a3-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="954a3-109">转到 %appdata%\microsoft\teams 并删除所有文件。</span><span class="sxs-lookup"><span data-stu-id="954a3-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="954a3-110">重新打开 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="954a3-110">Reopen Microsoft Teams.</span></span>
