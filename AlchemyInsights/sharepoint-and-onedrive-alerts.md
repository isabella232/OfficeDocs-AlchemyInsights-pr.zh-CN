---
title: 接收通知SharePoint OneDrive延迟
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: bd60159789bc4945c7f5e464fd1359e8fb8458cd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328428"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>接收通知SharePoint OneDrive延迟

- 如果 **来自多个文件或** 库的所有警报都延迟，请访问"服务运行状况 [](https://portal.office.com/adminportal/home?ref=/servicehealth)"仪表板，以检查所有警报/事件SharePoint或Exchange。
- 如果未 **传递来自特定文件或** 库的单个警报，则尝试删除并重新创建它。 请参阅[管理、查看或删除SharePoint警报以](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)重新创建警报。
- 检查电子邮件中的"垃圾邮件"文件夹。

**注意**：
- 无法向通讯组发送通知。 仅支持安全组和 O365 组。
- 无法自定义通知电子邮件模板。 您必须使用Microsoft Flow或SharePoint设计器工作流来实现这些目的。
