---
title: 发送到"垃圾邮件"文件夹的出站电子邮件
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
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096648"
---
# <a name="outbound-email-to-junk-email-folder"></a>发送到"垃圾邮件"文件夹的出站电子邮件

如果看到出站邮件被标记为"垃圾邮件"，请执行以下步骤：

- 如果尚未配置，请考虑 [配置出站垃圾邮件策略通知](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)。

- 使用 [邮件跟踪](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)查看出站邮件的事件值是否包含其他详细信息：**使用高风险传递池**。

  对于这些邮件，请检查邮件内容以查看可能被视为垃圾邮件的内容。 例如，签名有时会导致许多用户出现问题。

  如果你有多个标记为"垃圾邮件"的合法出站邮件示例，请打开一个支持票证，并要求支持代理将你的邮件提交为误报，以发送给我们的垃圾邮件分析师。 准备提供包括所有邮件头的示例邮件。
