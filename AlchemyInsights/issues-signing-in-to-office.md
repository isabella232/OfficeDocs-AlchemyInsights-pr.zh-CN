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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088026"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>应用中的空白登录Microsoft 365屏幕

若要解决此问题，请尝试执行以下操作：
- 安装适用于 Windows 和[Office](https://support.microsoft.com/help/4027667/windows-10-update) [的最新更新](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)。
- 重置Internet Explorer选项： 转到工具Internet 选项 高级重置 Internet Explorer 设置 (请注意，你将丢失自定义设置  >    >    >  ) ，然后再次尝试登录Office重置。
- 禁用Windows Defender 应用程序防护 (WDAG) 或任何类似的防火墙或防病毒程序：
    1. 在"控制面板"中，**转到"** 程序"，然后选择"**打开Windows或关闭"打开或关闭功能"。**
    2. 如果Windows Defender 应用程序防护，请尝试禁用它。<br/>
    **注意：** 您可能需要重新启动计算机。
- 确保 Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 插件未被任何应用程序或防火墙/防病毒程序阻止。
- [使用Office管理器](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)清除Windows凭据。<br/>
    **注意：** 2016 Office注册表路径已更改为 16.0。  (：\Software\Microsoft\Office\16.0\Common\Identity\)

有关详细信息，请参阅 Windows 10 上的更新到[Office 2016 内部版本 16.0.7967 后登录的连接Windows 10。](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)