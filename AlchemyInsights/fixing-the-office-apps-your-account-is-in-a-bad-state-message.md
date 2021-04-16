---
title: 修复 Microsoft 365 应用 你的帐户的状态消息错误
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812526"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>修复 Microsoft 365 应用"你的帐户状态错误"错误

若要修复此错误，请尝试在受影响的计算机上使用下列选项：

- 打开 Office 应用，选择"**文件**  >    >  **""帐户注销所有帐户"。** 使用具有有效许可证的用户帐户再次登录。 有关详细信息，请参阅 [Office 中的帐户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- [使用 Windows 凭据管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 清除 Office 凭据。<br>
  **注意：** Office 2016 的注册表路径已更改为 16.0。 例如，\Software\Microsoft\Office\16.0\Common\Identity\
- 如果在使用 Office 2013 连接到 Office 365 时发生错误，请 [为](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Office 客户端启用新式验证。

有关详细信息，请参阅如何排查无法登录 [Microsoft 365、Azure](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)或 Intune 的非浏览器应用。

