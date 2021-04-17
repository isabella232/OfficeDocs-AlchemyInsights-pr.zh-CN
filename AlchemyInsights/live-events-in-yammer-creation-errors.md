---
title: Yammer 实时事件创建错误
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825505"
---
# <a name="live-events-in-yammer-creation-errors"></a>Yammer 实时事件创建错误

**创建 Yammer 实时事件**

Yammer 将始终显示创建实时事件的选项。 在某些情况下，用户可能不符合创建实时事件的先决条件，并会在尝试创建实时事件时收到错误。 下面各项介绍了此问题的常见原因，并为最终用户提供解决方法。

**谁可以创建实时事件**
- Office 365 企业版 E1、E3 或 E5 许可证，或 Office 365 A3 或 A5 许可证。
- 在 Microsoft Teams 管理中心创建实时事件的权限。
- 在 Microsoft Stream 中创建实时事件的权限（适用于使用外部广播应用或设备制作的事件）。
- 组织中的正式团队成员身份（不能是来宾或来自其他组织）。
- 私人会议计划、屏幕共享、IP 会议共享、已在 Team 会议策略中打开。

**创建实时事件策略**

Yammer 遵循 Stream 的 Office 365 租户中设置的实时事件策略。 默认情况下，组织中的所有人均可创建实时事件。 管理员可能会[对此设置进行更改，这可能会阻止用户创建实时事件](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。 如果用户收到策略错误，请务必检查用户是否具有创建实时事件的权限。
