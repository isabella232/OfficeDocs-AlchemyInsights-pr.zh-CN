---
title: 2491 警报来自"由于租户或用户覆盖而传递的网络钓鱼"策略的电子邮件
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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999662"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>警报来自"由于租户或用户覆盖而传递的网络钓鱼"策略的电子邮件

名为"由于租户或用户覆盖而送达的网络钓鱼"的默认警报策略已推出给使用 Microsoft Defender 的租户，Office 365 P1 和 P2 许可证。 如果您收到此警报，以下是要调查的步骤：

1. 从警报消息中，单击 **"查看警报**"以转到安全与合规中心&警报"页面。

2. 选择警报以查看查看邮件列表或在资源管理器 **中查看邮件的选项**。  这两个选项都使你可以查看邮件的详细信息，其中包括邮件 ID。 请注意，威胁资源管理器链接将自动筛选与警报条件匹配的邮件。 你可能需要在威胁资源管理器中调整日期筛选器。

由于手动配置的覆盖，传送了网络钓鱼邮件：

- 用户设置的允许发件人或域。

- 管理员在反垃圾邮件策略中设置的允许发件人或域。

- 连接筛选器策略中允许的 IP 地址。

- 邮件流规则 (也称为传输规则) 配置为允许邮件使用的邮件流规则。

如果您认为邮件被错误地标记为网络钓鱼邮件，请使用 Outlook[报告邮件外接程序](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)将邮件示例提交给 Microsoft。
