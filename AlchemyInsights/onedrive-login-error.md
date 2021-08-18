---
title: OneDrive登录错误 AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112902"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive登录错误 AADSTS50011

如果在登录 OneDrive 应用时收到错误"AADSTS50011：请求中指定的回复 URL 与回复不匹配"，请检查以下内容：

你的OneDrive版本必须等于或大于版本 20.052.XXXX.XXXX。 To check your version， click on the blue OneDrive icon in the notification area， select **Help & 设置 > 设置 > About**.

网络可能会阻止到 g.live.com **和 oneclient.sfx.ms** **的流量**。 如果该流量被阻止，OneDrive无法自行更新。 与网络管理员合作，确保你有权访问这些 URL。 [对于使用](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)特定计划的客户，应Microsoft 365终结点。

如果需要手动获取当前版本的 OneDrive，请访问 [https://aka.ms/getonedrive](https://aka.ms/getonedrive) 。
