---
title: 密码日志
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523080"
---
# <a name="password-logs"></a><span data-ttu-id="de0d0-102">密码日志</span><span class="sxs-lookup"><span data-stu-id="de0d0-102">Password logs</span></span>

<span data-ttu-id="de0d0-103">**访问密码重置审核日志时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="de0d0-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="de0d0-104">若要解决有关访问密码重置审核日志的问题，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="de0d0-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="de0d0-105">确保你有权查看审核日志。</span><span class="sxs-lookup"><span data-stu-id="de0d0-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="de0d0-106">只有以下角色具有授权：</span><span class="sxs-lookup"><span data-stu-id="de0d0-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="de0d0-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="de0d0-107">Global administrator</span></span>
 - <span data-ttu-id="de0d0-108">安全管理员</span><span class="sxs-lookup"><span data-stu-id="de0d0-108">Security administrator</span></span>
 - <span data-ttu-id="de0d0-109">安全读者</span><span class="sxs-lookup"><span data-stu-id="de0d0-109">Security reader</span></span>

<span data-ttu-id="de0d0-110">**我想查看自最初部署起的所有密码重置审核事件**</span><span class="sxs-lookup"><span data-stu-id="de0d0-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="de0d0-111">过去 30 天的报告中最多存储了 120，000 个密码重置/注册事件。</span><span class="sxs-lookup"><span data-stu-id="de0d0-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="de0d0-112">下载 CSV 时，此最大限制适用于 UI。</span><span class="sxs-lookup"><span data-stu-id="de0d0-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="de0d0-113">PowerShell 提供 100 万个事件。</span><span class="sxs-lookup"><span data-stu-id="de0d0-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="de0d0-114">有关详细信息，请参阅以下链接：</span><span class="sxs-lookup"><span data-stu-id="de0d0-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="de0d0-115">Azure AD 报表和事件 API 中的自助密码重置事件</span><span class="sxs-lookup"><span data-stu-id="de0d0-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="de0d0-116">如何使用 PowerShell 快速下载密码重置注册事件</span><span class="sxs-lookup"><span data-stu-id="de0d0-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="de0d0-117">**我想了解有关密码重置报告功能更多信息**</span><span class="sxs-lookup"><span data-stu-id="de0d0-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="de0d0-118">在 "用户和组"下，在 Azure 门户中检查谁正在注册或重置 Azure AD 密码重置 **重置**。</span><span class="sxs-lookup"><span data-stu-id="de0d0-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="de0d0-119">有关详细信息，请参阅以下链接：</span><span class="sxs-lookup"><span data-stu-id="de0d0-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="de0d0-120">密码重置报告概述</span><span class="sxs-lookup"><span data-stu-id="de0d0-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="de0d0-121">如何在 Azure 门户中查看密码重置报告</span><span class="sxs-lookup"><span data-stu-id="de0d0-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="de0d0-122">Azure AD 报表和事件 API 中的自助密码重置事件</span><span class="sxs-lookup"><span data-stu-id="de0d0-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="de0d0-123">如何使用 PowerShell 快速下载密码重置注册事件</span><span class="sxs-lookup"><span data-stu-id="de0d0-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


