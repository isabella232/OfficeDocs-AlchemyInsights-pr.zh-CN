---
title: 1385-Office-365-警报-策略
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664016"
---
# <a name="alert-policies"></a>警报策略

Microsoft 365 security & 合规性中心提供了 [默认通知策略](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) ，这些策略将触发 Office 365 企业版或 OFFICE 365 美国政府 E1/G1、E3/G3 或 E5/G5 订阅的组织的警报。 因此，管理员可能会收到由 Office365Alerts@microsoft.com 发送的通知电子邮件通知，其中包含 "低严重性警报： *警报策略的名称*" 等主题行。 当常见活动触发警报时，将发送警报通知，例如当用户执行以下操作时：

- 创建转发电子邮件的收件箱规则。
- 为其邮箱分配权限。
- 在 SharePoint 文件共享中共享或删除大量文件。
- 创建电子数据展示搜索和导出搜索结果。

查看警报并对其执行操作：

1. 转到 [安全 & 合规性中心](https://protection.office.com) 并登录。
2. 单击 "**警报**  >  **查看警报**"。
3. 单击某个通知可显示包含有关该警报的信息的飞出页面。

您可以对通知执行操作，例如 [删除可疑的收件箱规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)。 或者，可以通过单击 "通知弹出窗口" 页上的 " **解决** " 直接关闭该警报。

有关配置和管理通知策略的详细信息，请参阅  [本文](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)。

**重要说明**：通知来自 Microsoft 的电子邮件通知决不会要求您执行以下操作：

- 提供密码
- 验证帐户的安全详细信息
- 重新对自己进行身份验证

如果您收到这样的电子邮件，则它不是由 Microsoft 发送的，应被视为仿冒欺诈。 如果发生这种情况，请 [将其报告给 Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。