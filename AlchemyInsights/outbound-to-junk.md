---
title: 出站电子邮件至垃圾邮件文件夹
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769173"
---
# <a name="outbound-email-to-junk-email-folder"></a>出站电子邮件至垃圾邮件文件夹

如果要查看标记为垃圾邮件的出站邮件，请执行以下步骤：

- 如果还未配置，请考虑 [配置出站垃圾邮件策略通知](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)。

- 使用 [邮件跟踪](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) 查看出站邮件是否具有其他详细信息的事件值 **垃圾邮件** ： **使用高风险传递池**。

  对于这些邮件，请检查邮件内容以查看可能被视为垃圾邮件的内容。 例如，签名有时可能会导致许多用户出现问题。

  如果您有多个将被标记为垃圾邮件的合法出站邮件的示例，请打开支持票证，并请求支持代理将您的邮件作为误报提交给垃圾邮件分析员。 准备提供包含所有邮件头的示例邮件。
