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
# <a name="create-a-group"></a>创建群组

本主题介绍组创建。

**创建组的权限**

确保你有权创建新组。 全局管理员可在 Azure 门户或访问面板中禁用组创建。 可能需要管理员来新建组或授予你适当的权限。

**管理组创建权限**

1. 全局管理员可以管理组创建权限 (出于安全原因) 或在 Azure 门户或访问面板中创建的 Office 365 组，方法为选择"用户可以在 Azure 门户中创建安全组"或"用户可以在 Azure 门户中创建 Office 365 组"选项（"所有组常规 (设置  >  **) "** 中）。
2. 如果你拥有 Azure Active Directory P1 Premium 许可证，还可以限制组创建以选择一组用户。

**禁用新 Office 365 组成员的欢迎通知**

可以通过在 Powershell 中将 **UnifiedGroupWelcomeMessageEnabled** 设置为 False 来禁用向已添加到 Office 365 组的用户发送的欢迎通知。 在此处了解有关此设置 [，](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)。

