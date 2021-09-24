---
title: 从 Microsoft 名称服务器更改回管理自己的 DNS 记录
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481837"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>从 Microsoft 名称服务器更改回管理自己的 DNS 记录

你之前将 NS 记录更改为指向 Microsoft (ns1.bdm.microsoftonline.com)，但现在已决定管理自己的 DNS 记录：

在域注册机构的网站上，将名称服务器更改回注册机构或以前的设置。 如果不熟悉 DNS，请联系域注册机构的支持人员。 请注意，名称服务器更改最多可能需要 48 小时才能传播。 

1. 在 Microsoft 365 管理门户中，转到“**设置**” > [“**域**”](https://admin.microsoft.com/Adminportal/Home#/Domains)，选中域旁边的复选框，然后选择“**管理 DNS**”。 

2. 在向导中，选择“**添加自己的 DNS 记录**”并完成向导。 此操作会更改 DNS 的管理方式，然后允许添加支持所选服务所需的自定义 DNS 记录。

或者，如果已将名称服务器记录更改为 Microsoft 并拥有网站，则可以为网站添加 DNS 记录，而不是将名称服务器改回。 有关详细信息，另请参阅 [更新 DNS 记录以便利用当前的托管提供商继续托管网站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)。


