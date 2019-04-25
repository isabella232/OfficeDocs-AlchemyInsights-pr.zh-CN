---
title: 1336 RecoverableItems 文件夹已满
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389073"
---
# <a name="the-recoverable-items-folder-is-full"></a>"可恢复的项目" 文件夹已满

对于 Office 365 中的 Exchange Online 邮箱, "可恢复的项目" 文件夹的默认存储限制为 30 GB。 如果将邮箱置于诉讼保留、电子数据展示保留或分配到 Office 365 保留策略, 则 "可恢复的项目" 文件夹的存储限制将自动增加到 100 GB。

当 "可恢复的项目" 文件夹达到存储限制时, 邮箱功能将受到以下几种影响:

- 用户不能删除邮箱中的项目。

- 托管文件夹助理无法基于保留标记或托管文件夹设置删除项目。

- 对于启用了单个项目恢复或置于保留状态的邮箱, "写入时复制" 页面保护过程无法维护用户编辑的项目的版本。

- 对于启用了邮箱审核日志记录的邮箱, 不能将邮箱审核日志条目保存在 "可恢复的项目" 文件夹的 "审核" 子文件夹中。

对于不处于保留状态的邮箱, 管理员可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell 中的命令删除 "可恢复的项目" 文件夹中的项目。 有关详细信息，请参阅下列主题： 

- [搜索和删除邮件](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [搜索-邮箱](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

对于处于保留状态的邮箱, 管理员必须先删除保留, 然后才能从 "可恢复的项目" 文件夹中删除项目。 有关详细信息, 请参阅[在保留时, 删除基于云的邮箱的 "可恢复的项目" 文件夹中的项目](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。

为了帮助防止 "可恢复的项目" 文件夹变满, 管理员可以增加保留邮箱的 "可恢复的项目" 文件夹的存储限制, 并设置将项目从 "可恢复的项目" 文件夹移动到用户存档的邮箱保留策略信箱. 请参阅[增大保留邮箱的可恢复邮件配额](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
