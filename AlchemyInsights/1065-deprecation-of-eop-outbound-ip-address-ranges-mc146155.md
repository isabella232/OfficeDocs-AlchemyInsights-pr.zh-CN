---
title: 1065 否决的 EOP 出站 IP 地址 rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277320"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation 的 EOP 出站的 IP 地址范围

我们已检测到 （如果不更正 2018 年 10 月 26，由） 可能会中断到您的内部或外部目标的邮件流贵组织的潜在问题。为以前交流，若要简化 IP 地址范围管理，我们合并用于发送和接收 Office 365 以外的电子邮件的 Exchange Online Protection (EOP) IP 地址范围。我们的分析表明以下一项或多个源外部电子邮件或您已配置邮件流连接器的目标不接受来自 IP 地址范围显示[此处](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的连接。
  
操作之前年 10 月 26 以确保这些源和目标将接受连接到并从所有[发布 EOP IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。
  
有关此更改的详细信息，请参阅邮件中心文章[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。
  
 **注意**： 如果您以前使用的终结点更新的 HTML，XML，and RSS 通过 IP 或 URL 发布，还应迁移到新的 web 服务用于自动执行这些类型的更新。有关详细信息，请参阅[Office 365 终结点类别和 Office 365 IP 地址、 web 服务 URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
  

