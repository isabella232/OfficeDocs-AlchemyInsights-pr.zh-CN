---
title: Microsoft 365 中的 2681 攻击模拟器
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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325061"
---
# <a name="attack-simulator-in-microsoft-365"></a>攻击模拟器Microsoft 365

- 你缺少攻击模拟器吗？ 攻击模拟器需要 **Microsoft Defender Office 365计划 2** 或 **Office 365 企业版 E5。** 攻击模拟器 **不包含在** Microsoft Defender for Office 365计划 1、Office 365 企业版 E3 或任何 Microsoft 365 商业应用版订阅中。

- 用于启动模拟攻击的帐户需要全局管理员或安全管理员权限以及 MFA (多重) 。 有关攻击模拟器要求的详细信息，请参阅 [本主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。

- 有关暴力 **密码攻击模拟** 的重要信息：

  - 如果目标帐户已启用 MFA 并且正确猜测了密码，则该帐户不会 (第二个身份验证因素将) 。

  - 密码文件不能大于 10 MB。 每行使用一个密码，在列表中最后 (个) 后包含一个空行。

- 有关网络钓鱼附加模拟 **的** 重要信息：

  - 根据设计，无法为网络钓鱼登录服务器 **URL 提供自定义值**。

  - 如果收件人使用 ["](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 启用报告邮件"加载项将邮件报告为网络钓鱼邮件，则可能不会收到邮件提示 (因为这是模拟的攻击) 。

- 报告：模拟攻击完成后，你可以单击" **攻击详细信息** "查看报告。

- 有关攻击模拟器中的详细说明和新功能，请参阅攻击模拟器[Microsoft 365。](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
