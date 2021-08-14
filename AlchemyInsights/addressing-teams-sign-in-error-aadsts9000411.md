---
title: 解决 Teams 登录错误 AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953001"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>解决 Teams 登录错误 AADSTS9000411

登录 Microsoft Teams 时，可能会收到以下错误：**抱歉，在 AADSTS9000411 中登录时遇到问题：请求的格式不正确。参数“login_hint”重复。**

若要解决此问题，请确保你的 Microsoft Teams 客户端已更新。 有关更新客户端的详细信息，请参阅 [更新 Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

如果由于某种原因无法更新客户端，注销客户端将清除大部分缓存数据。 但是，如果在注销/登录后仍遇到问题，请退出 Teams 并执行以下操作来清除客户端缓存：
1. 关闭 Microsoft Teams。
2. 转到 %appdata%\microsoft\teams 并删除所有文件。
3. 重新打开 Microsoft Teams。
