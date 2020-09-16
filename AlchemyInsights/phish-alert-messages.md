---
title: 2491通知电子邮件来自 "由于租户或用户替代而发送的网络钓鱼" 策略
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728601"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>通知来自 "由于租户或用户替代的网络钓鱼传递" 策略的电子邮件

一个名为 "由于租户或用户替代而发送的网络钓鱼" 的默认通知策略已通过 Office 365 ATP P1 和 P2 许可证推出给租户。 如果你收到此通知，请查看以下步骤：

1. 在警告消息中，单击 " **查看通知** " 以转到安全 & 合规性中心中的 " **通知** " 页面。

2. 选择警报以查看 **查看邮件列表** 的选项或 **查看资源管理器中的邮件**。 这两个选项都将您带到邮件的详细信息，其中包括邮件 ID。 请注意，威胁资源管理器链接将自动筛选符合警报条件的邮件。 您可能需要在威胁资源管理器中调整日期筛选器。

由于手动配置的替代，已传递网络钓鱼邮件：

- 用户设置的允许发件人或域。

- 由管理员在反垃圾邮件策略中设置的允许发件人或域。

- 连接筛选器策略中允许的 IP 地址。

- 邮件流规则 (也称为传输规则) ，配置为允许中的邮件。

如果您认为邮件被错误地标记为网络钓鱼，请使用 Outlook [报告邮件外接程序](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) 将邮件示例提交给 Microsoft。
