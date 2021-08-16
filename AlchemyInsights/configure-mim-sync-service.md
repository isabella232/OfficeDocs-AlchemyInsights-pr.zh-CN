---
title: 配置 MIM 同步服务
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978475"
---
# <a name="configure-mim-sync-service"></a>配置 MIM 同步服务

Microsoft Identity Manager （MIM） 同步服务是 MIM 的一个组件。 它是一种集中式本地服务，为具有多个本地目录和数据库的组织存储和集成信息。 如果在 MIM 的最近更新中解决了你的问题，或者该问题是在下节中所提及的其他问题之一，则可能在 MIM 同步后解决你的问题。

**建议的步骤**

1. 确保使用的是 MIM 同步的最新更新，并检查 [MIM 同步发行说明](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) 以确定该问题是否已在更新中得到解决。
2. 如果问题出现在 Generic LDAP、Generic SQL、Lotus Domino 或 Web Services 连接器上，请确保使用的是最新更新的 [通用连接器](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)。
3. 如果 MIM 同步运行因错误而停止，请参阅 [运行错误代码](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) 表以确认潜在原因。
4. 如果运行停止时出现 **“extension-dll-exception”**，请单击这些字样打开 **“连接器空格对象属性”** 窗口，然后单击 **“堆叠跟踪...”** 更多关于根本原因的信息，如 [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)中所述。
5. 如果密码更改通知服务 (PCNS) 组件在密码同步期间事件日志中报告 **错误 6025** ，请查看 [PCNS 报告错误 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx) 的故障排除指南。
6. 如果与 FIM 服务管理代理完全同步速度较慢，请检查TempDB 的 **自动增加** 设置，如 [解决完全同步速度慢或挂起故障](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)中所述。
7. 如果在使用 FIM 服务管理代理时遇到停用服务器的错误，并出现 failed-creation-via-web-services，请参阅 [支持信息: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services)以了解原因概述。

