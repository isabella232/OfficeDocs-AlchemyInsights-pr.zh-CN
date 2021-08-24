---
title: Microsoft Teams 组织结构图中未显示用户图片
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467365"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Microsoft Teams 组织结构图中未显示用户图片

如果组织中一个或多个人员在组织结构图中缺少其个人资料照片，则 **ShowInAddressLists** 设置可能设置为 **False**：

1. 转到 Microsoft 365 管理中心 >[**活动用户**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)，然后选择缺少照片的用户。 
1. 选择"**邮件**"选项卡，并确保"**在全局地址列表中显示**"设置为"**是**"。 

如果将 **ShowInAddressLists** 设置为 **"是"** 不起作用，请检查以下各项：

- 用户可能在 Exchange 收件人列表中隐藏。 有关详细信息，请参阅[管理 Exchange Online 中的地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)。 
- 用户可能在 Azure Active Directory 地址列表中隐藏。 有关详细信息，请参阅 [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)。 
