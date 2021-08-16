---
title: 修复Microsoft 365帐户状态错误消息
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068226"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>修复Microsoft 365应用"帐户状态错误"错误

若要修复此错误，请尝试在受影响的计算机上使用下列选项：

- 打开Office 应用，选择"**文件**  >    >  **""帐户注销所有帐户"。** 使用具有有效许可证的用户帐户再次登录。 有关详细信息，请参阅 [Office 中的帐户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- [使用Office管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)清除Windows凭据。<br>
  **注意：** 2016 Office注册表路径已更改为 16.0。 例如，\Software\Microsoft\Office\16.0\Common\Identity\
- 如果在使用 Office 365 2013 连接到 Office 时发生错误，请为 Office[](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)客户端启用新式验证。

有关详细信息，请参阅如何排查无法登录 [Microsoft 365、Azure](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)或 Intune 的非浏览器应用。

