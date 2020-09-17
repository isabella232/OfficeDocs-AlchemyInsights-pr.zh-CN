---
title: 1065 EOP 出站 IP 地址的弃用 rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806785"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>弃用 EOP 出站 IP 地址范围

我们检测到您的组织可能存在 (如果未在26年10月26日纠正的问题，2018) 可能会破坏您的内部部署或外部目标的邮件流。 如前所述，为了简化 IP 地址范围管理，我们正在合并 Exchange Online Protection (EOP) IP 地址范围，用于在 Microsoft 365 之外发送和接收电子邮件。 我们的分析表明，在邮件流连接器中配置的一个或多个外部电子邮件源或目标无法接受 [此处](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)显示的 IP 地址范围的连接。

在10月26日之前行动，以确保这些源和目标将接受与所有 [发布的 EOP IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的连接。

有关此更改的详细信息，请参阅消息中心发布 [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或 [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。

**注意**：如果以前使用过通过 HTML、XML 和用于终结点更新的 RSS 来发布 IP 或 URL，则还应迁移到新的 web 服务以自动执行这些类型的更新。 有关详细信息，请参阅 [microsoft 365 终结点类别和 microsoft 365 IP 地址和 URL web 服务](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
