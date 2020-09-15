---
title: 登录到 Microsoft 365 应用程序时出现问题
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695169"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>解决 Microsoft 365 应用程序 "计算机的受信任的平台模块无法正常运行" 消息

若要修复此错误，请使用以下步骤：

- 安装最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。
- 使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **注意：** Office 2016 的注册表路径已更改为16.0。  (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)
- 尝试 [用户恢复过程](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 以修复受信任的平台模块 (TPM) 故障。
- 使用以下步骤设置 EnableADAL = 0：  
    1. 右键单击 Windows "开始" 按钮，选择 " **运行**"，键入 " **regedit**"，然后选择 **"确定"**。
    2. 选择 **"是"** 以允许注册表编辑器对你的设备进行更改。
    3. 在注册表编辑器中，将 **EnableADAL** 的 DWORD 值添加到 HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity. 下的设置为 **0** 。

有关详细信息，请参阅在 [Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。