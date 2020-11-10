---
title: OneDrive 登录错误 AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947477"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="27648-102">OneDrive 登录错误 AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="27648-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="27648-103">如果您收到错误 "AADSTS50011：在登录到 OneDrive 应用时，请求中指定的答复 URL 与答复不匹配，请检查以下各项：</span><span class="sxs-lookup"><span data-stu-id="27648-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="27648-104">你的 OneDrive 版本必须等于或大于版本20.052。XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX.</span><span class="sxs-lookup"><span data-stu-id="27648-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="27648-105">若要检查版本，请单击通知区域中的蓝色 OneDrive 图标，选择 " **帮助" & 设置 "> 设置" >** "。</span><span class="sxs-lookup"><span data-stu-id="27648-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="27648-106">你的网络可能会阻止到 **g.live.com** 和 **oneclient.sfx.ms** 的流量。</span><span class="sxs-lookup"><span data-stu-id="27648-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="27648-107">如果该流量被阻止，OneDrive 将无法自我更新。</span><span class="sxs-lookup"><span data-stu-id="27648-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="27648-108">与您的网络管理员合作，以确保您有权访问这些 Url。</span><span class="sxs-lookup"><span data-stu-id="27648-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="27648-109">对于使用 Microsoft 365 计划的客户，[这些终结点](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)应是可访问的。</span><span class="sxs-lookup"><span data-stu-id="27648-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="27648-110">如果需要手动获取 OneDrive 的最新版本，请访问 [https://aka.ms/getonedrive](https://aka.ms/getonedrive) 。</span><span class="sxs-lookup"><span data-stu-id="27648-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
