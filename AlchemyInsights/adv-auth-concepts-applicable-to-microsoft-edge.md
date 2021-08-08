---
title: 适用于用户的高级身份验证Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934355"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>适用于用户的高级身份验证Microsoft Edge

下面是适用于以下应用程序的高级身份验证Microsoft Edge：

**主动身份验证**

启用[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621)策略时，Microsoft Edge将尝试通过策略主动验证登录Microsoft 服务。 它定期使用联机服务检查更新的清单，其中包含管理主动身份验证的配置。

优点：主动身份验证支持对关键服务（如"新建选项卡Office）进行身份验证。 此外，必应用作搜索引擎，则主动身份验证可提高地址栏的性能，并帮助生成个性化的搜索结果以满足业务需求。

**Windows HelloCredUI for NTLM Authentication**

如果单一登录 (SSO) 在网站尝试通过 NTLM 或协商机制登录用户时不可用，则此功能将允许用户与网站共享操作系统凭据，并通过使用 Windows Hello Cred UI 满足身份验证质询。 此登录流程将仅出现在 Windows 10 中，并且仅适用于在 NTLM 或协商质询期间未获取 SSO 的用户。

**使用保存的密码自动登录**

在密码中保存Microsoft Edge用户可以启用自动登录到已保存凭据的网站。 用户可以在密码管理器中打开或 edge://settings/passwords 此功能，并且您可以在密码管理器 [策略中对其进行](https://go.microsoft.com/fwlink/?linkid=2134622) 配置。
