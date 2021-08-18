---
title: 域状态 - 未选择任何服务
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326567"
---
# <a name="domain-status---no-services-selected"></a>域状态 - 未选择任何服务

未 **选择** 任何服务意味着你尚未选择任何 Microsoft 365 服务（如 Exchange Online、Skype for Business 或 Intune）和移动设备管理Microsoft 365用于自定义域。 如果在本地将 Exchange 混合 (Exchange与 Exchange Online) 或外部垃圾邮件筛选一Exchange且没有任何Microsoft 服务，可以忽略此邮件。 域运行状况状态仅适用于直接连接到服务的域。

若要为域选择服务：

1. From **设置**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home)， check the box next to the domain with the status message **No services selected**.
1. 选择 **"管理 DNS"** 以启动域设置向导。
    - 如果选择" **添加自己的 DNS 记录"，** 请确保在系统提示时选择服务。 高级选项 下可能提供了 **更多服务**。
    - 如果选择"**允许 Microsoft 添加 DNS** 记录"或"更多 **选项**""为我设置联机服务"，将自动建议和  >  选择所有可用服务。
1. 继续执行向导以完成 DNS 设置和服务选择。
 
有关设置域的其他帮助，请参阅添加 [DNS 记录以连接域](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。

