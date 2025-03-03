---
title: SharePoint 和 OneDrive 中 Office 文件的敏感性标签的限制
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: 376c0293c325a725c117d54bb0f15b0146b9224c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332807"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>SharePoint 和 OneDrive 中 Office 文件的敏感性标签的限制

在为 SharePoint 和 OneDrive 中的 Office 文件启用敏感标签时，要注意一些要求和限制，其中包括:

- 当文件包含 PowerQuery 数据、自定义插件存储的数据或自定义 XML 部分时，SharePoint 和 OneDrive 无法处理来自 Office 桌面应用程序的一些标记和加密的文件。
- SharePoint 和 OneDrive 不会对已使用 Azure 信息保护 (AIP) 标签加密的现有文件自动应用敏感度标签。若要对加密的文件应用敏感度标签，请执行以下操作： 
    - 请确保 AIP 标签已迁移并发布到 Microsoft 365 合规中心。
    - 下载带有标记的文件，然后将其上传到原来的 SharePoint 或 OneDrive 位置。
- 对于加密文档，不支持打印。

有关限制的其他细节，请参阅 [为 SharePoint 和 OneDrive 中的 Office 文件启用敏感标签](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)。
