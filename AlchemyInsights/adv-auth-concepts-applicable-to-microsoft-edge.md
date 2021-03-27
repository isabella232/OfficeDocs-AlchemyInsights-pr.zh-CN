---
title: 适用于 Microsoft Edge 的高级身份验证概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398542"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>适用于 Microsoft Edge 的高级身份验证概念

以下是适用于 Microsoft Edge 的高级身份验证概念：

**主动身份验证**

启用 [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 策略后，Microsoft Edge 将尝试通过 Microsoft 服务主动验证登录用户的身份。 它定期使用联机服务检查更新的清单，其中包含管理主动身份验证的配置。

优点：主动身份验证支持对关键服务（如 Office 新选项卡页）进行身份验证。 此外，如果将必应用作搜索引擎，则主动身份验证可改进地址栏的性能，并帮助生成个性化的搜索结果以满足业务需求。

**用于 NTLM 身份验证的 Windows Hello CredUI**

如果单一登录 (SSO) 在网站尝试通过 NTLM 或协商机制登录用户时不可用，则此功能将允许用户与网站共享操作系统凭据，并通过使用 Windows Hello Cred UI 满足身份验证质询。 此登录流程将仅在 Windows 10 中显示，并且仅适用于在 NTLM 或协商质询期间未获取 SSO 的用户。

**使用保存的密码自动登录**

在 Microsoft Edge 中保存密码的用户可以启用自动登录到已保存凭据的网站。 用户可以在密码管理器中打开或 edge://settings/passwords 此功能，并且您可以在密码管理器 [策略中对其进行](https://go.microsoft.com/fwlink/?linkid=2134622) 配置。
