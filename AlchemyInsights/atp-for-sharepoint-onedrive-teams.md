---
title: 适用于 SharePoint、OneDrive 和 Microsoft Teams 的 ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715551"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>适用于 SharePoint、OneDrive 和 Microsoft Teams 的 ATP

按照以下步骤启用高级威胁防护：

1. 转到 [https://protection.office.com](https://protection.office.com) 并使用全局管理员帐户或安全管理员帐户登录。

2. 在 " **威胁管理**" 下方的左侧导航窗格中，选择 " **策略** \> **安全附件**"。

3. 选择 " **为 SharePoint、OneDrive 和 Microsoft 团队启用 ATP**"。

4. [创建活动通知策略](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) 以在检测到恶意文件时接收通知。

有关完整说明，请参阅本 [主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)。

**注意**：根据设计，ATP 不会扫描 SharePoint Online、OneDrive for Business 或 Microsoft 团队中的每个文件。 通过使用共享活动、来宾活动和威胁信号识别恶意文件的进程，异步扫描文件。 有关详细信息，请参阅本 [主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。
