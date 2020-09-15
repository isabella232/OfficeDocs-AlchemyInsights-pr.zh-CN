---
title: 团队4c7 错误
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700193"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="0e0b8-102">Microsoft 团队中的4c7 错误</span><span class="sxs-lookup"><span data-stu-id="0e0b8-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="0e0b8-103">出现此错误的原因是 Microsoft 团队需要表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="0e0b8-104">在部署 Active Directory 联合身份验证服务 (AD FS) 时，默认情况下不会为 intranet 启用表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="0e0b8-105">如果 Windows 集成身份验证失败，系统会提示您使用表单身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="0e0b8-106">若要解决此问题，请使用 AD FS Microsoft 管理控制台 (MMC) 管理单元在具有 Active Directory 的本地副本的计算机上启用表单身份验证。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="0e0b8-107">为此，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="0e0b8-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="0e0b8-108">在导航窗格中，浏览到 " **身份验证策略**"。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="0e0b8-109">在 "详细信息" 窗格的 " **操作** " 下，选择 " **编辑全局主身份验证**"。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="0e0b8-110">在 " **Intranet** " 选项卡上，选择 " **表单身份验证**"。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="0e0b8-111">选择 **"确定"** (或 " **应用**) "。</span><span class="sxs-lookup"><span data-stu-id="0e0b8-111">Select **OK** (or **Apply**).</span></span>