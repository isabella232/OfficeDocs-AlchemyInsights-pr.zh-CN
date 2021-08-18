---
title: 通过 Microsoft 365 中继电子邮件
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324352"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>设置多功能设备或应用程序以发送电子邮件

若要了解有关选项和步骤的详细信息，请参阅[如何设置多功能设备或应用程序以使用 Microsoft 365 发送电子邮件](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。
  
如果你的设备或应用程序最近停止工作，最常见的问题有：

- **使用 SMTP 身份验证客户端提交身份验证时出现的相关错误** 我们最近对 SMTP 身份验证的工作方式进行了一些更改。 有关如何解决问题的详细信息，请参阅[修复使用 Microsoft 365 或 Office 365 发送电子邮件的打印机、扫描仪和 LOB 应用程序的问题](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)的身份验证失败部分。
- **我们只接受 TLS 1.2 版本，同时与 Office 365 建立安全连接** 如果你使用的是安全连接 (TLS)，请确保应用程序设备支持 TLS 1.2。 有关详细信息，请参阅[在 Office 365 和 Office 365 GCC 中准备 TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)。
 
有关其他问题和解决方案，请参阅[修复使用 Microsoft 365 或 Office 365 发送电子邮件的打印机、扫描仪和 LOB 应用程序的问题](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)。

要查看受影响的设备，请转到 [SMTP 身份验证客户端报表](https://protection.office.com/mailflow/dashboard)。

**注意**：Exchange Online 不适用于批量邮件方案。若要发送批量商业电子邮件（例如，客户新闻稿），应使用专用于这些服务的第三方提供商。
