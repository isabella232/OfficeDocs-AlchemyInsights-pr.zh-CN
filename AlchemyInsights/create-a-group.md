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
# <a name="create-a-group"></a>创建组

本主题介绍组创建。

**创建组的权限**

确保您有权创建新组。 全局管理员可以在 Azure 门户或访问面板中禁用组创建。 您可能需要管理员为您创建新组，或者为您提供适当的权限。

**管理组创建权限**

1. 全局管理员可以管理组创建权限 (以实现与安全相关的原因) 或在 azure 门户或访问面板中创建的 Office 365 组、选择 "用户可以在 azure 门户中创建安全组" 或 "**所有组** 中的用户可以在 azure 门户中创建 office 365 组" 选项。) 的所有 (组中的 "用户可以创建 Office 组" 选项  >  ****。
2. 如果你拥有 Azure Active Directory P1 高级许可证，也可以限制组创建以选择一组用户。

**禁用新 Office 365 组成员的欢迎通知**

向添加到 Office 365 组的用户发送的欢迎通知可以通过在 Powershell 中将 **UnifiedGroupWelcomeMessageEnabled** 设置为 False 来禁用。 请 [在此处](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)了解此设置。

