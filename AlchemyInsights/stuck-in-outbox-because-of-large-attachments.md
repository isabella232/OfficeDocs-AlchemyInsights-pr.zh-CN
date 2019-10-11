---
title: 由于大型附件导致发件箱中的卡
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441296"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>修复发件箱中卡住的邮件

我们建议您从[Microsoft 支持和恢复助手](https://diagnostics.office.com/#/)工具中运行["我遇到了问题发送、接收或查找电子邮件问题"](https://aka.ms/SaRA-OutlookSendReceive)这一方案开始。

当邮件滞留在发件箱中时，最可能的原因是：
- 大型附件。
- 未启用 "**连接后立即发送**" 选项。

要删除大附件，请执行以下操作： 

1. 在 Outlook 中，选择 "**发送/接收** > **脱机工作**"。 
2. 在导航窗格中，选择 **"发件箱"**。 在此处，您可以执行以下操作： 
    - 删除邮件（选择它，然后选择 "**删除**"）。
    - 将邮件拖到 "草稿" 文件夹中，双击以打开它，然后删除附件，选择它，然后选择 "**删除**"。
3. 如果收到指示 Outlook 尝试传输邮件的错误，请关闭 Outlook。 可能需要几分钟才能退出。 如果 Outlook 未关闭，请按 Ctrl + Alt + Delete，然后选择 "**启动任务管理器**"。 在任务管理器中，选择 "**进程**" 选项卡，向下滚动到 "setup.exe"，然后选择 "**结束进程**"。
4. Outlook 关闭后，重新启动它并重复步骤2和3。 
5. 删除附件后，请单击 "脱机**发送/接收** > **工作**" 以恢复联机工作。 

当您单击 "**发送**"，但未连接时，邮件也会陷入发件箱中。 单击 "**发送/接收**" 并查看 "**脱机工作**" 按钮。 如果是蓝色，则断开连接。 选择它以进行连接（该按钮变为白色），然后单击 "**全部发送**"。
 
若要**在连接时立即启用 Send**：
 
- 选择 "**高级**" "**文件** > **选项** >  "。
在 "**发送和接收**" 部分，选择 "**连接后立即发送**"，然后选择 **"确定"**。
 
有关完整的详细信息，请参阅：
- [视频：发送或删除卡住的电子邮件](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [在 Outlook 中手动启动发送/接收操作之前，电子邮件将一直保留在 "发件箱" 文件夹中](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
