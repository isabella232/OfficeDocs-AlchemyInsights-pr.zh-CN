---
title: 修复 Microsoft 365 应用你的帐户处于错误状态消息
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744535"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>修复 Microsoft 365 应用程序 "你的帐户处于错误状态" 错误

若要修复此错误，请在受影响的计算机上尝试以下选项：

- 打开 Office 应用程序，选择 "**文件**  >  **帐户**注销  >  **所有帐户**"。 使用具有有效许可证的用户帐户再次登录。 有关详细信息，请参阅 [Office 中的帐户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br>
  **注意：** Office 2016 的注册表路径已更改为16.0。 例如，\Software\Microsoft\Office\16.0\Common\Identity\
- 如果使用 Office 2013 连接到 Office 365 时出现错误，请为 Office 客户端 [启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 。

有关详细信息，请参阅 [如何排查无法登录到 Microsoft 365、Azure 或 Intune 的非浏览器应用程序的问题](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)。

