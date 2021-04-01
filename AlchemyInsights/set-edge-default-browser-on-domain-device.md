---
title: 将 Microsoft Edge 设置为加入域的设备上的默认浏览器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426776"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>将 Microsoft Edge 设置为加入域的设备上的默认浏览器

将 Microsoft Edge 设置为默认浏览器： 

1. [创建默认关联配置文件](https://go.microsoft.com/fwlink/?linkid=2132437)并将其存储在本地或网络共享上。

1. 打开组策略编辑器，然后转到“**计算机配置**” > “**管理模板**” > “**Windows 组件**” > “**文件资源管理器**”。

1. 选择“**设置默认关联配置文件**”。

1. 选择“**策略设置**”，然后选择“**启用**”。

1. 在“**选项**”下，输入默认关联配置文件的位置，然后选择“**确定**”。
