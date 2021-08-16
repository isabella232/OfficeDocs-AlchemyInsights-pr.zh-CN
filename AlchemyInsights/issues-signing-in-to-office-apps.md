---
title: 登录应用Microsoft 365问题
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
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028030"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>修复Microsoft 365"抱歉，组织的另一个帐户已登录"消息

若要修复此错误，请使用以下步骤：

- 使用"访问工作或学校"Windows 设置 >除受影响的帐户外 **，删除所有工作帐户**。
- [使用Office管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)清除Windows凭据。<br/>
    **注意：** 2016 Office注册表路径已更改为 16.0。  (：\Software\Microsoft\Office\16.0\Common\Identity\)
- 打开一Office 应用，选择"**文件**  >  **""帐户**  >  **注销"。** 然后使用具有有效许可证的用户帐户登录。 有关详细信息，请参阅[Office 中的账户](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 对于 Mac，参见[无法登录至 Office 2016 for Mac 应用](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。

有关详细信息，请参阅"抱歉，您的组织中的另一个帐户已在此计算机上登录["。Office。](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)