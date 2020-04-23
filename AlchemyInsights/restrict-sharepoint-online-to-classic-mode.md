---
title: 将 SharePoint Online 限制为经典模式
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742459"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>将 SharePoint Online 限制为经典模式

有些组织仍需要经典模式体验。 虽然没有计划在粒度级别删除经典模式，但不再可能将整个组织（租户）限制为列表和库的经典模式。

管理员可通过以下方式来管理采用经典模式的各个列表和库，具体方法是使用我们在以下级别提供的具体选择退出开关：

- site collection
- 网站
- list
- 图书馆

此外，使用新式不支持的某些功能和自定义项的列表仍将自动切换到经典模式。

从2019年4月1日起，禁用租户级别的过程退出新式列表，库将在5月31日（2019）开始并继续。  由于租户自愿退出，以经典模式的列表和库将自动移动到新式。

如果需要经典模式，请[参阅此处的详细信息和](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)PnP Powershell 说明，[此处](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)介绍了可用于今天使用经典模式体验的选项和工具。
