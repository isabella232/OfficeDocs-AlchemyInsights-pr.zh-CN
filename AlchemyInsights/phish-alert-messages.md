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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316348"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>警报来自"由于租户或用户覆盖而传递的网络钓鱼"策略的电子邮件

在具有 Microsoft Defender for Office 365 P1 和 P2 许可证的组织中，可以使用名为 **"** 由于租户或用户覆盖而送达的网络钓鱼"的默认警报策略。 如果您收到此警报，以下是要调查的步骤：

1. 在警报消息中，单击 **"查看警报**"以转到警报门户中的Microsoft 365 Defender页。

2. 选择警报以查看查看邮件列表或在资源管理器 **中查看邮件的选项**。  这两个选项都使你可以查看邮件的详细信息，其中包括邮件 ID。 请注意，威胁资源管理器链接将自动筛选与警报条件匹配的邮件。 你可能需要在威胁资源管理器中调整日期筛选器。

由于手动配置的覆盖，传送了网络钓鱼邮件：

- 用户设置的允许发件人或域。
- 管理员在反垃圾邮件策略中设置的允许发件人或域。
- 连接筛选器策略中允许的 IP 地址。
- 邮件流规则 (也称为传输规则) 配置为允许邮件使用的邮件流规则。

如果认为邮件被错误地标记为网络钓鱼，请使用管理员提交将邮件报告[](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)给 Microsoft。

用户可以使用报告[邮件外接程序或](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)报告网络钓鱼外接程序Outlook向 Microsoft 提交邮件示例。
