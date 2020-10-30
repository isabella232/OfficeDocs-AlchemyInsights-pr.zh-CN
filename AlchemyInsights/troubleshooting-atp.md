---
title: Microsoft Defender for Office 365 的故障排除
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801433"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Microsoft Defender for Office 365 的故障排除

- 您是否注意到邮件传递延迟？ 在 ATP 安全附件策略中使用 [动态传递](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) 选项。 这将有助于避免邮件延迟，同时防止收件人受到恶意文件的攻击。

- 是否要向 Microsoft 报告误报或漏报？ 使用此 [链接](https://www.microsoft.com/wdsi/filesubmission/) 提交文件以进行分析。

- 您是否知道您可以为组织内的收件人之间发送的内部电子邮件启用安全链接保护？ 请按以下步骤操作：

  1. 转到 [https://protection.office.com](https://protection.office.com) 并使用全局管理员帐户或安全管理员帐户登录。

  2. 在 " **威胁管理** " 下方的左侧导航窗格中，选择 " **策略** \> **安全链接** "。

  3. 在 " **适用于整个组织的策略** " 部分中，选择该策略，然后单击 " **编辑** "。

  4. 在 " **设置** " 下，启用 " **对组织中发送的邮件应用安全链接** "。
