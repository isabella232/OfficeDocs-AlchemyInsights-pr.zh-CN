---
title: Microsoft 365 中的2681攻击模拟器
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759209"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365 中的攻击模拟器

- 是否缺少攻击模拟器？ 攻击模拟器需要 **Office 365 高级威胁防护计划 2 (ATP Plan 2) ** 或 **Office 365 企业版 E5**。 "攻击模拟器" **不** 包含在 Office 365 高级威胁防护计划 1 (ATP Plan 1) 、Office 365 企业版 E3 或任何 Microsoft 365 应用程序的商业版订阅。

- 您用于启动模拟攻击的帐户需要全局管理员或安全管理员权限，且多重身份验证 (MFA) 。 有关攻击模拟器要求的详细信息，请参阅 [本主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。

- 有关 **强力密码** 攻击模拟的重要须知：

  - 如果目标帐户已启用 MFA 且密码被正确猜出，则该帐户不会显示为 "已损坏" (第二个身份验证因子将不完全) 。

  - 密码文件不能大于 10 MB。 每行使用一个密码，并在列表中的最后一个密码后面 (回车) 加上一个空行。

- 了解有关 **Spear 的网络钓鱼** 附加模拟的重要事项：

  - 根据设计，不能为 **网络钓鱼登录服务器 URL**提供自定义值。

  - 如果收件人使用 " [启用报告邮件" 加载项](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 将邮件报告为网络钓鱼，则您可能不会收到邮件 (的通知，因为这是模拟的攻击) 。

- 报告：在模拟的攻击完成之后，您可以单击 " **攻击详细信息** " 来查看报告。

- 有关攻击模拟器的详细说明和新功能，请参阅 [Microsoft 365 中的攻击模拟器](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。
