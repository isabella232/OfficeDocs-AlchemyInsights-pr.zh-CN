---
title: 1336 RecoverableItems 文件夹已满
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061746"
---
# <a name="the-recoverable-items-folder-is-full"></a>"可恢复的项目"文件夹已满

对于Exchange Online邮箱，"可恢复的项目"文件夹的默认存储限制为 30 GB。 如果邮箱处于诉讼保留、电子数据展示保留或分配给保留策略，则"可恢复的项目"文件夹的存储限制会自动增加到 100 GB。

当"可恢复的项目"文件夹达到存储限制时，邮箱功能会以下列方式受到影响：

- 用户无法从邮箱中删除项目。

- 托管文件夹助理无法基于保留标记或托管文件夹设置删除项目。

- 对于启用了单个项目恢复或置于保留状态邮箱，写入时复制页面保护过程无法维护用户编辑的项目的版本。

- 对于已启用邮箱审核日志记录的邮箱，审核日志"可恢复的项目"文件夹的"审核"子文件夹中保存任何邮箱项目。

对于未保留的邮箱，管理员可以使用 PowerShell 中的Exchange Online删除"可恢复 `Search-Mailbox -SearchDumpsterOnly -DeleteContent` 的项目"文件夹中的项目。 有关详细信息，请参阅下列主题：

- [搜索和删除邮件](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

对于保留的邮箱，管理员必须删除保留，然后才能从"可恢复的项目"文件夹中删除项目。 有关详细信息，请参阅删除保留的基于云的邮箱的"可恢复的项目" [文件夹中的项目](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。

为了帮助防止"可恢复的项目"文件夹已满，管理员可以为保留的邮箱增加"可恢复的项目"文件夹的存储限制，并设置将项目从"可恢复的项目"文件夹移动到用户的存档邮箱的邮箱保留策略。 请参阅 [增加保留邮箱的可恢复邮件配额](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
