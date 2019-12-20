---
title: 团队4c7 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795976"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="8ddb0-102">Microsoft 团队中的4c7 错误</span><span class="sxs-lookup"><span data-stu-id="8ddb0-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="8ddb0-103">出现此错误的原因是 Microsoft 团队需要表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="8ddb0-104">当您部署 Active Directory 联合身份验证服务（AD FS）时，默认情况下不会为 intranet 启用表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="8ddb0-105">如果 Windows 集成身份验证失败，系统会提示您使用表单身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="8ddb0-106">若要解决此问题，请使用具有 Active Directory 本地副本的计算机上的 AD FS Microsoft 管理控制台（MMC）管理单元启用表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="8ddb0-107">要实现这一点，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="8ddb0-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="8ddb0-108">在导航窗格中，浏览到 "**身份验证策略**"。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="8ddb0-109">在 "详细信息" 窗格的 "**操作**" 下，选择 "**编辑全局主身份验证**"。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="8ddb0-110">在 " **Intranet** " 选项卡上，选择 "**表单身份验证**"。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="8ddb0-111">选择 **"确定"** （或 "**应用**"）。</span><span class="sxs-lookup"><span data-stu-id="8ddb0-111">Select **OK** (or **Apply**).</span></span>