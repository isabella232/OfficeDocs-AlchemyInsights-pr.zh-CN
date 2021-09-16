---
title: 用户图片仍显示在 Microsoft Teams 组织结构图中
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334354"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>用户图片仍显示在 Microsoft Teams 组织结构图中

如果组织中一个或多个人员已被禁用或删除，并且其个人资料照片仍显示在组织结构图中，则 **ShowInAddressLists** 设置可能设置为 False： 

1. 转到 Microsoft 365 管理中心 >“[活动用户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)”，然后选择仍显示的照片的用户。 
1. 选择“**邮件**”选项卡，并确保“**在全局地址列表中显示**”设置为“**否**”。

如果将 **ShowInAddressLists** 设置为“**否**”不起作用，请检查以下各项： 

- 用户可能在 Exchange 收件人列表中显示。 有关详细信息，请参阅[管理 Exchange Online 中的地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)。 
- 用户可能在 Azure Active Directory 地址列表中显示。 有关详细信息，请参阅 [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)。 