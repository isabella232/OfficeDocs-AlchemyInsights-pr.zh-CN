---
title: 126 在 OWA 中找不到邮箱错误？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056480"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>在 Outlook 网页版中遇到“邮箱未找到”错误？

如果您使用的是 Outlook 网页版并且由于错误而找不到 **Mailbox，** 则用于连接到 Outlook 网页版 的帐户没有 Exchange Online 许可证，因此，没有邮箱与该帐户关联。 管理员按照以下步骤操作，可以向帐户分配许可证：

1. 打开Microsoft 365 管理中心 [转到](https://portal.office.com/adminportal/home#/homepage)**"用户"** 部分下的"活动用户"，然后选择看到错误的用户。

2. 在打开的用户页中，转到"许可证和应用"部分，选择相应的 **"** 位置"值，并分配包含 Exchange Online (的许可证，以查看其详细信息) 。 完成后，单击“**保存更改**”。

在某些情况下，如果许可证已分配给用户帐户，则删除和重新分配许可证有助于解决问题，并正确在系统中进行预配： 

- 查看你的 M365 订阅Exchange Online (（如果有）是否) 订阅当前且尚未过期。

一旦确保你的订阅未过期并且向用户帐户分配了有效的许可证，设置许可证可能需要 24 小时，因此你可能必须等待问题解决。 有关详细信息，请参阅分配 [和管理许可证](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)。