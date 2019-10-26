---
title: 305增加存档邮箱大小
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36661790"
---
# <a name="increase-the-archive-mailbox-size"></a>增加存档邮箱大小

Office 365 根据分配给用户帐户的许可证[限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)存档邮箱的大小。 当存档邮箱达到其允许大小的90% 时，用户将收到电子邮件通知。 当存档邮箱达到其大小限制时，用户将无法将更多项目移至存档邮箱。 一旦达到大小限制，Office 365 将不会增加存档邮箱的大小。 相反，用户可以执行以下操作来释放存档邮箱中的空间：

- 使用 Outlook 将项目导出到 .pst 文件。

- 删除存档邮箱中的项目。

Office 365 提供了 Office 365 企业版 E3 和 E5 许可证的**无限制存档**。 管理员必须先启用此功能，存档邮箱才能达到其最大大小。 启用无限期存档时，最长可能需要30天，才能将可用空间添加到存档邮箱中。 因此，我们建议管理员验证存档邮箱中的可用空间，以便用户可以在扩展时继续使用存档邮箱。 有关详细信息，请参阅[office 365 中的无限制存档概述](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)和[在 Office 365 中启用无限制存档](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)。

有关从 Outlook 访问存档邮箱的详细信息，请参阅[访问自动扩展存档中的项目的 Outlook 要求](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)。 若要配置自动将项目移动到存档邮箱的保留策略，请参阅为[Office 365 组织中的邮箱设置存档和删除策略](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)。

**注意**： Exchange 2010 上的主邮箱不支持自动扩展存档。
