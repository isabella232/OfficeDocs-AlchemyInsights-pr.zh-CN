---
title: 1065 EOP 出站 IP 地址的弃用 rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404811"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>弃用 EOP 出站 IP 地址范围

我们检测到您的组织存在潜在问题 (如果未在10月26日纠正, 2018) 可能会破坏您的内部部署或外部目标的邮件流。 如前所述, 为了简化 IP 地址范围管理, 我们正在合并用于在 Office 365 外部发送和接收电子邮件的 Exchange Online Protection (EOP) IP 地址范围。 我们的分析表明, 在邮件流连接器中配置的一个或多个外部电子邮件源或目标无法接受[此处](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)显示的 IP 地址范围的连接。

在10月26日之前行动, 以确保这些源和目标将接受与所有[发布的 EOP IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的连接。

有关此更改的详细信息, 请参阅消息中心发布[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。

**注意**: 如果以前使用过通过 HTML、XML 和用于终结点更新的 RSS 来发布 IP 或 URL, 则还应迁移到新的 web 服务以自动执行这些类型的更新。 有关详细信息, 请参阅[office 365 终结点类别和 Office 365 IP 地址和 URL web 服务](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
