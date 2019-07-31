---
title: 登录 Office 应用程序时出现问题
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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938144"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>修复 Office 应用程序 "计算机的受信任的平台模块未正常运行" 消息

若要修复此错误, 请尝试以下操作:

- 安装最新的[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。
- 使用 Windows 凭据管理器[清除 Office 凭据](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **注意:** Office 2016 的注册表路径已更改为16.0。 (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- 尝试[用户恢复过程](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)以修复受信任的平台模块 (TPM) 故障。
- 使用以下步骤设置 EnableADAL = 0:  
    1. 右键单击 Windows "开始" 按钮, 选择 "**运行**", 键入 " **regedit**", 然后选择 **"确定"**。
    2. 选择 **"是"** 以允许注册表编辑器对你的设备进行更改。
    3. 在注册表编辑器中, 将**EnableADAL**的 DWORD 值添加到 HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity. 下的设置为**0** 。

有关详细信息, 请参阅在[Windows 10 上更新到 Office 2016 生成16.0.7967 后登录中的连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。