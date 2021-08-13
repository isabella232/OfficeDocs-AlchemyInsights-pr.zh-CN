---
title: 打开或保存文件时出错
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
- "9000583"
- "2685"
ms.openlocfilehash: 13a75338e3784d3df2ec93e8096380f85494317b7161040c7ad60ad830f9211d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978079"
---
# <a name="resolve-errors-opening-or-saving-word-files"></a>解决打开或保存 Word 文件时出错

如果在打开或保存 Word 文档时遇到问题，请尝试执行以下操作：

- [安装Office更新](https://support.office.com/article/2ab296f3-7f03-43a2-8e50-46de917611c5)。 有关最新更新Office，请参阅[最新更新](https://docs.microsoft.com/officeupdates/office-updates-msi)。
- [排查 Word 中损坏的文档。](https://docs.microsoft.com/office/troubleshoot/word/damaged-documents-in-word)
- [修复Office应用程序](https://support.office.com/Article/Repair-an-Office-application-7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。
- 如果文档包含修订，请使用 [Word](https://docs.microsoft.com/office/troubleshoot/word/word-stops-responding) 中的建议，如果跟踪更改或注释过多，将减慢或停止响应，以解决问题。

如果收到类似以下错误之一的错误，请使用注册表策略设置阻止文件时Office中的错误消息[中的建议](https://docs.microsoft.com/office/troubleshoot/settings/file-blocked-in-office)：

- 你正在尝试打开注册表策略设置阻止的文件。
- 你正尝试打开的文件类型 **\<File Type\>** 已被“信任中心”的“文件阻止”设置阻止。
- 你正在尝试打开由以前版本的 Microsoft Office 创建的文件。 注册表策略设置已阻止此文件在该版本中打开。
- 你正在尝试保存注册表策略设置阻止的文件。
- 您试图在信任中心保存已被"文件阻止"设置阻止的文件类型。

如果从 SharePoint 或 OneDrive 文档库打开 Office 文件时遇到问题，请尝试以下操作：

- 请检查[OneDrive、OneDrive for Business 和 SharePoint 中无效的文件名和文件类型](https://support.office.com/article/64883a5d-228e-48f5-b3d2-eb39e07630fa)中的文件限制，以确保文件受到支持。 
- [删除 Office 文档缓存](https://support.office.com/article/b1d3765e-d71b-4bb8-99ca-acd22c42995d
)。 

有关详细信息，请参阅[修复打开 SharePoint 库中的文档时出现的问题](https://support.office.com/article/31329fa1-4ad0-47fc-95d8-bb0c5b12a536)。