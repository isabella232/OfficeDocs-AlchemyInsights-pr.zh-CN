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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986881"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>修复Microsoft 365应用的"您的计算机的受信任平台模块无法正常工作"消息

若要修复此错误，请使用以下步骤：

- 安装适用于 Windows 和[Office](https://support.microsoft.com/help/4027667/windows-10-update) [的最新更新](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)。
- [使用Office管理器](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer)清除Windows凭据。<br/>
    **注意：** 2016 Office注册表路径已更改为 16.0。  (：\Software\Microsoft\Office\16.0\Common\Identity\)
- 尝试用户 [恢复过程以](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 修复 TPM (受信任的) 模块。
- 使用以下步骤设置 EnableADAL = 0：  
    1. 右键单击"Windows"按钮，选择"运行"，键入 **regedit，** 然后选择"确定 **"。** 
    2. 选择 **"** 是"以允许注册表编辑器对设备进行更改。
    3. 在注册表编辑器中，将 **EnableADAL** 的 DWORD 值设置为 **0，** 在"HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity"下。

有关详细信息，请参阅 Windows 10 上的更新到[Office 2016 内部版本 16.0.7967 后登录的连接Windows 10。](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)