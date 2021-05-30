---
title: 终结点 DLP 未部署到用户的设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694801"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="51840-102">终结点 DLP 未部署到用户的设备</span><span class="sxs-lookup"><span data-stu-id="51840-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="51840-103">如果终结点数据丢失防护 (DLP) 设置尚未应用于用户的设备，请确认你满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="51840-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="51840-104">Windows 10 x64 内部版本 1809 或更高版本已安装在设备上。</span><span class="sxs-lookup"><span data-stu-id="51840-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="51840-105">反恶意软件客户端版本 4.18.2009.7 或更高版本已安装。</span><span class="sxs-lookup"><span data-stu-id="51840-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="51840-106">设备满足以下条件 **之一**：</span><span class="sxs-lookup"><span data-stu-id="51840-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="51840-107">已建立 Azure Active Directory (Azure AD) 联接</span><span class="sxs-lookup"><span data-stu-id="51840-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="51840-108">已建立混合 Azure AD 联接</span><span class="sxs-lookup"><span data-stu-id="51840-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="51840-109">已完成 AAD 注册</span><span class="sxs-lookup"><span data-stu-id="51840-109">AAD registered</span></span>

- <span data-ttu-id="51840-110">若要执行策略操作，请确保终结点设备上已安装 Microsoft Chromium Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="51840-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="51840-111">有关部署终结点 DLP 的其他要求，请参阅[终结点数据丢失防护入门](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="51840-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>