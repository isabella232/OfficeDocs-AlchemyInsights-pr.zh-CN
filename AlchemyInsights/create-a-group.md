---
title: 创建组
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086233"
---
# <a name="create-a-group"></a><span data-ttu-id="c2ee2-102">创建组</span><span class="sxs-lookup"><span data-stu-id="c2ee2-102">Create a group</span></span>

<span data-ttu-id="c2ee2-103">本主题介绍组创建。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-103">This topic describes group creation.</span></span>

<span data-ttu-id="c2ee2-104">**创建组的权限**</span><span class="sxs-lookup"><span data-stu-id="c2ee2-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="c2ee2-105">确保您有权创建新组。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="c2ee2-106">全局管理员可以在 Azure 门户或访问面板中禁用组创建。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="c2ee2-107">您可能需要管理员为您创建新组，或者为您提供适当的权限。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="c2ee2-108">**管理组创建权限**</span><span class="sxs-lookup"><span data-stu-id="c2ee2-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="c2ee2-109">全局管理员可以管理组创建权限 (以实现与安全相关的原因) 或在 azure 门户或访问面板中创建的 Office 365 组、选择 "用户可以在 azure 门户中创建安全组" 或 "**所有组** 中的用户可以在 azure 门户中创建 office 365 组" 选项。) 的所有 (组中的 "用户可以创建 Office 组" 选项  >  \*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="c2ee2-110">如果你拥有 Azure Active Directory P1 高级许可证，也可以限制组创建以选择一组用户。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="c2ee2-111">**禁用新 Office 365 组成员的欢迎通知**</span><span class="sxs-lookup"><span data-stu-id="c2ee2-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="c2ee2-112">向添加到 Office 365 组的用户发送的欢迎通知可以通过在 Powershell 中将 **UnifiedGroupWelcomeMessageEnabled** 设置为 False 来禁用。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="c2ee2-113">请 [在此处](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)了解此设置。</span><span class="sxs-lookup"><span data-stu-id="c2ee2-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

