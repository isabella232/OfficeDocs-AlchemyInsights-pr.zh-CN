---
title: Microsoft 365 管理中心中的报告不显示可读的用户名
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327804"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 管理中心中的报告不显示可读的用户名

Microsoft 365 管理中心中的报告不显示用户名，而是显示字母数值，例如 B2BC6C15BB9FCDEA71E5CD302D228CC8。

这是预期行为，并已在消息中心沟通（MC275344，已于 2021 年 8 月 3 日发布）。 

如果全局管理员的组织隐私实践允许，则全局管理员可为其租户还原此更改并显示可识别的用户信息。若要为租户还原此更改，请执行以下操作：

1. 在管理中心，转到“**设置**” > “**组织设置**” > [“**服务**”](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )，然后选择“**报表**”。 
1. 在“**选择如何显示用户信息**”下，选择“**在报表中显示可识别的用户信息**”，然后重新运行该报表。