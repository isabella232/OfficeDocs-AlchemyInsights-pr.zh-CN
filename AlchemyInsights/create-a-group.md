---
title: 创建群组
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816335"
---
# <a name="create-a-group"></a><span data-ttu-id="668be-102">创建群组</span><span class="sxs-lookup"><span data-stu-id="668be-102">Create a group</span></span>

<span data-ttu-id="668be-103">本主题介绍组创建。</span><span class="sxs-lookup"><span data-stu-id="668be-103">This topic describes group creation.</span></span>

<span data-ttu-id="668be-104">**创建组的权限**</span><span class="sxs-lookup"><span data-stu-id="668be-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="668be-105">确保你有权创建新组。</span><span class="sxs-lookup"><span data-stu-id="668be-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="668be-106">全局管理员可在 Azure 门户或访问面板中禁用组创建。</span><span class="sxs-lookup"><span data-stu-id="668be-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="668be-107">可能需要管理员来新建组或授予你适当的权限。</span><span class="sxs-lookup"><span data-stu-id="668be-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="668be-108">**管理组创建权限**</span><span class="sxs-lookup"><span data-stu-id="668be-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="668be-109">全局管理员可以管理组创建权限 (出于安全原因) 或在 Azure 门户或访问面板中创建的 Office 365 组，方法为选择"用户可以在 Azure 门户中创建安全组"或"用户可以在 Azure 门户中创建 Office 365 组"选项（"所有组常规 (设置  >  **) "** 中）。</span><span class="sxs-lookup"><span data-stu-id="668be-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="668be-110">如果你拥有 Azure Active Directory P1 Premium 许可证，还可以限制组创建以选择一组用户。</span><span class="sxs-lookup"><span data-stu-id="668be-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="668be-111">**禁用新 Office 365 组成员的欢迎通知**</span><span class="sxs-lookup"><span data-stu-id="668be-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="668be-112">可以通过在 Powershell 中将 **UnifiedGroupWelcomeMessageEnabled** 设置为 False 来禁用向已添加到 Office 365 组的用户发送的欢迎通知。</span><span class="sxs-lookup"><span data-stu-id="668be-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="668be-113">在此处了解有关此设置 [，](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="668be-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

