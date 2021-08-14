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
ms.openlocfilehash: ba46da6d67bbfd602d8e5f3fa03d0e607ba3243ad4b9b592b09b606c73fa8f44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921753"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>将 Microsoft Edge 设置为加入域的设备上的默认浏览器

将 Microsoft Edge 设置为默认浏览器： 

1. [创建默认关联配置文件](https://go.microsoft.com/fwlink/?linkid=2132437)并将其存储在本地或网络共享上。

1. 打开组策略编辑器，然后转到“**计算机配置**” > “**管理模板**” > “**Windows 组件**” > “**文件资源管理器**”。

1. 选择“**设置默认关联配置文件**”。

1. 选择“**策略设置**”，然后选择“**启用**”。

1. 在“**选项**”下，输入默认关联配置文件的位置，然后选择“**确定**”。
