---
title: 数据位置
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627836"
---
# <a name="data-location"></a>数据位置

您可以查看管理中心的 Office 365 租户的位置或通过 PowerShell 连接到 Exchange Online。


**管理中心：**
1. 登录到[管理中心](https://admin.microsoft.com/Adminportal/Home)。
2. 选择 "**设置** > **组织配置文件**"。
3. 在 "**数据位置**" 下，选择 "**查看详细信息**"。


**PowerShell**
1. 使用 Windows PowerShell 连接到 Exchange Online。
2. 执行[OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet 可显示租户的属性列表。 
3. 查看 OrganizationId 属性。

当您具有 EXO 和 SPO 的数据位置时，可以确定您的[数据所在位置](https://products.office.com/where-is-your-data-located)可能使用的其他服务的数据位置。