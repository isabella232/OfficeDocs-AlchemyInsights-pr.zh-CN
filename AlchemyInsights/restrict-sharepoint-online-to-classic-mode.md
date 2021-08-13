---
title: 将 SharePoint Online 限制为经典模式
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958791"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>将 SharePoint Online 限制为经典模式

某些组织仍然需要经典模式体验。 尽管没有计划在粒度级别删除经典模式，但不再可能将整个组织 (租户) 列表和库的经典模式。

管理员将具有以下选项，以使用我们在以下级别提供的粒度选择退出开关在经典模式下管理各个列表和库：

- 网站集
- 网站
- list
- 库

此外，使用新式版本不支持的某些功能和自定义项的列表仍将自动切换到经典模式。

从 2019 年 4 月 1 日起，从 2019 年 5 月 31 日起，将启动禁用租户级别选择退出新式列表和库的过程，并持续到 2019 年 5 月 31 日。  由于租户选择退出而进入经典模式的列表和库将自动转移到新式。

如果需要经典模式，请在此处查看详细信息，[](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)并在此处查看 PnP [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) Powershell 说明，其中介绍了现在可用于使用经典模式体验的选项和工具。
