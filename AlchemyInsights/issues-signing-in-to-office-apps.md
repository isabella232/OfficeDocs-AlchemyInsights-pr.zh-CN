---
title: 登录 Microsoft 365 应用时的问题
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833065"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>修复 Microsoft 365 应用"抱歉，组织的另一个帐户已登录"消息

若要修复此错误，请使用以下步骤：

- 使用 Windows 设置或访问工作或学校 ，删除> **帐户，受影响的帐户除外**。
- [使用 Windows 凭据管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 清除 Office 凭据。<br/>
    **注意：** Office 2016 的注册表路径已更改为 16.0。  (：\Software\Microsoft\Office\16.0\Common\Identity\)
- 打开 Office 应用，选择"**文件**  >  **""帐户**  >  **注销"。** 然后使用具有有效许可证的用户帐户登录。 有关详细信息，请参阅[Office 中的账户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 对于 Mac，参见[无法登录至 Office 2016 for Mac 应用](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。

有关详细信息，请参阅 Office 中的"抱歉，您的组织中的另一个帐户已[在此计算机上登录"。](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)