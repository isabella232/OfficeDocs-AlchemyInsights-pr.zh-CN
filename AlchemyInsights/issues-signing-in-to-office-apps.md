---
title: 登录到 Microsoft 365 应用程序时出现问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579927"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>修复 Microsoft 365 应用程序 "抱歉，你的组织中的另一个帐户已登录" 消息

若要修复此错误，请使用以下步骤：

- 使用 Windows 设置 >**访问工作或学校**，删除除受影响帐户之外的所有工作帐户。
- 使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **注意：** Office 2016 的注册表路径已更改为16.0。 （Ex： \Software\Microsoft\Office\16.0\Common\Identity\)
- 打开 Office 应用程序，选择 "**文件**  >  **帐户**  >  **注销**"。然后使用具有有效许可证的用户帐户登录。 有关详细信息，请参阅[Office 中的账户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 对于 Mac，参见[无法登录至 Office 2016 for Mac 应用](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。

有关详细信息，请参阅[Office 中的 "抱歉，你的组织中的另一个帐户已在此计算机上登录"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)。