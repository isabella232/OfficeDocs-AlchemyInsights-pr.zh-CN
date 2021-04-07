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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597433"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>还原已删除的 Microsoft 365 组

可以在删除后 30 天内还原已删除的 Microsoft 365 组或 Microsoft Teams。

1. 转到 [Microsoft 365 管理](https://aka.ms/RestoreDeletedGroup) 中心登录并列出已删除的组和团队。

    **注意：** 使用分配给租户管理员或组管理员角色的帐户登录。

1. 选择要还原的已删除的 Microsoft 365 组/Teams，然后单击"**还原组"。**

    如果由于 SMTP 地址冲突而无法还原组，请使用以下命令查找导致冲突的对象并删除 SMTP 地址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **注意：** 在某些情况下，可能需要 24 小时才能还原组及其所有数据。

    有关详细信息，或了解如何使用 PowerShell 还原组，请参阅还原 [已删除的 Microsoft 365 组](https://go.microsoft.com/fwlink/?linkid=867802)。