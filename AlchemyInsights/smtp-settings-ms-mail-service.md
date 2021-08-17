---
title: Microsoft 365 邮件服务的 SMTP 设置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107149"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Microsoft 365 邮件服务的 SMTP 设置

以下是 Microsoft 365 邮件服务的 SMTP 设置：

**服务器**：smtp.office365.com </br>
**端口**：587 </br>
**加密**：STARTTLS（目前仅支持 TLS 1.2 版本）。 请确保应用程序或设备支持 TLS 1.2） </br>
**用户名**：Office 365 地址（例如 example@yourdomain.com） </br>
**密码**：Office 365 密码 </br>
**身份验证**：必需 </br>
**发送限制**：每天 10，000 封电子邮件 </br>

有关 POP 和 IMAP 设置，请参阅[POP、IMAP 和 SMTP 设置](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)。
 
若要了解使用 Microsoft 365 和步骤中继电子邮件的选项，请参阅 [ 如何设置多功能设备或应用程序以使用 Microsoft 365 或 Office 365 发送电子邮件](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365) 。