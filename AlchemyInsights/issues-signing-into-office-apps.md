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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832993"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>修复 Microsoft 365 应用"您的计算机的受信任平台模块无法正常工作"消息

若要修复此错误，请使用以下步骤：

- 安装 Windows [和](https://support.microsoft.com/help/4027667/windows-10-update) Office 的最新 [更新](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)。
- [使用 Windows 凭据管理器](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) 清除 Office 凭据。<br/>
    **注意：** Office 2016 的注册表路径已更改为 16.0。  (：\Software\Microsoft\Office\16.0\Common\Identity\)
- 尝试用户 [恢复过程以](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 修复 TPM (受信任的) 模块。
- 使用以下步骤设置 EnableADAL = 0：  
    1. 右键单击 Windows"开始"按钮，选择"**运行"，** 键入 **regedit**，然后选择"确定 **"。**
    2. 选择 **"** 是"以允许注册表编辑器对设备进行更改。
    3. 在注册表编辑器中，将 **EnableADAL** 的 DWORD 值设置为 **0，** 在"HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity"下。

有关详细信息，请参阅 [Windows 10 上的 Office 2016 内部版本 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)更新后登录的连接问题。