---
title: 182请运行 SaRA 以诊断和解决 Outlook 身份验证问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802011"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="069f2-102">使用 SaRA 诊断和解决 Outlook 身份验证问题</span><span class="sxs-lookup"><span data-stu-id="069f2-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="069f2-103">**注意**：请查看是否已为你的组织启用 [安全默认设置](https://aka.ms/securitydefaults) 。</span><span class="sxs-lookup"><span data-stu-id="069f2-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="069f2-104">如果你的租户是在10月21日之后创建2019的，并且你的 Outlook 反复要求你提供密码，则你的租户中可能启用了 **安全默认设置** 。</span><span class="sxs-lookup"><span data-stu-id="069f2-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="069f2-105">强烈建议使用 Outlook 在受影响的计算机上 [始终询问我的密码](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) 诊断，以解决 outlook 不断提示输入密码的问题。</span><span class="sxs-lookup"><span data-stu-id="069f2-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="069f2-106">此 [SaRA](https://diagnostics.office.com/#/) 诊断将执行自动检查，并返回可用于解决任何检测到的问题的可能解决方案。</span><span class="sxs-lookup"><span data-stu-id="069f2-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
