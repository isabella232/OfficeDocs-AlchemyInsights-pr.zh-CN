---
title: 还原已删除的Microsoft 365组
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959016"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>还原已删除的Microsoft 365组

可以在删除后Microsoft 365 30 Microsoft Teams还原已删除的组或组。

1. 转到[Microsoft 365 管理中心以](https://aka.ms/RestoreDeletedGroup)登录到你已删除的组和团队的列表。

    **注意：** 使用分配给租户管理员或组管理员角色的帐户登录。

1. 选择要还原的Microsoft 365组/Teams，然后单击"还原 **组"。**

    如果由于 SMTP 地址冲突而无法还原组，请使用以下命令查找导致冲突的对象并删除 SMTP 地址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **注意：** 在某些情况下，可能需要 24 小时才能还原组及其所有数据。

    有关详细信息，或了解如何使用 PowerShell 还原组，请参阅还原已删除Microsoft 365[组](https://go.microsoft.com/fwlink/?linkid=867802)。