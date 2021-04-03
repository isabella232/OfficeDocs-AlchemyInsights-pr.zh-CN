---
title: 还原已删除的 Microsoft 365 组
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505672"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>还原已删除的 Microsoft 365 组

可以在删除后 30 天内还原已删除的 Microsoft 365 组或 Microsoft Teams。

1. 若要登录到 Microsoft 365 管理中心并列出已删除的组和团队，请转到 [Microsoft 365 管理中心](https://aka.ms/RestoreDeletedGroup)。

    **注意：** 使用分配给租户管理员或组管理员角色的帐户登录。

1. 选择要还原的已删除的 Microsoft 365 组/Teams，然后单击"**还原组"。**

    如果由于 SMTP 地址冲突而无法还原组，请使用以下命令查找导致冲突的对象并删除 SMTP 地址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **注意：** 在某些情况下，可能需要 24 小时才能还原组及其所有数据。

    有关详细信息，或了解如何使用 PowerShell 还原组，请参阅还原 [已删除的 Microsoft 365 组](https://go.microsoft.com/fwlink/?linkid=867802)。