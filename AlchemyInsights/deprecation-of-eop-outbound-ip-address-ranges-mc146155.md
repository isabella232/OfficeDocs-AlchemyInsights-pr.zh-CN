---
title: 1065 弃用 EOP 出站 IP 地址范围MC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031252"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 出站 IP 地址范围弃用

我们检测到您的组织存在一个潜在的问题，即 (如果未在 2018 年 10 月 26 日之前进行纠正) 可能会中断到内部部署或外部目标的邮件流。 如前所述，为了简化 IP 地址范围管理，我们正在合并 Exchange Online Protection (EOP) IP 地址范围，用于发送和接收 Microsoft 365 外部的电子邮件。 我们的分析表明，在邮件流连接器中配置的一个或多个外部电子邮件源或目标不接受来自此处所示的 IP 地址范围 [的连接](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。

在 10 月 26 日前采取行动，以确保这些源和目标接受与所有已发布 [的 EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)地址的连接。

有关此更改详细信息，请参阅消息中心文章[MC146155、MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)或[MC149274。](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274) [](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)

**注意**：如果你之前通过 HTML、XML 和 RSS 为终结点更新使用了 IP 或 URL 发布，则还应迁移到新的 Web 服务以自动执行这些类型的更新。 有关详细信息，请参阅终结点Microsoft 365[和Microsoft 365 IP 地址和 URL Web 服务](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
