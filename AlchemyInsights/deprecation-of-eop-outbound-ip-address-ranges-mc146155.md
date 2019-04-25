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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="9e534-102">弃用 EOP 出站 IP 地址范围</span><span class="sxs-lookup"><span data-stu-id="9e534-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="9e534-103">我们检测到您的组织存在潜在问题 (如果未在10月26日纠正, 2018) 可能会破坏您的内部部署或外部目标的邮件流。</span><span class="sxs-lookup"><span data-stu-id="9e534-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="9e534-104">如前所述, 为了简化 IP 地址范围管理, 我们正在合并用于在 Office 365 外部发送和接收电子邮件的 Exchange Online Protection (EOP) IP 地址范围。</span><span class="sxs-lookup"><span data-stu-id="9e534-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="9e534-105">我们的分析表明, 在邮件流连接器中配置的一个或多个外部电子邮件源或目标无法接受[此处](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)显示的 IP 地址范围的连接。</span><span class="sxs-lookup"><span data-stu-id="9e534-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9e534-106">在10月26日之前行动, 以确保这些源和目标将接受与所有[发布的 EOP IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的连接。</span><span class="sxs-lookup"><span data-stu-id="9e534-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9e534-107">有关此更改的详细信息, 请参阅消息中心发布[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。</span><span class="sxs-lookup"><span data-stu-id="9e534-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="9e534-108">**注意**: 如果以前使用过通过 HTML、XML 和用于终结点更新的 RSS 来发布 IP 或 URL, 则还应迁移到新的 web 服务以自动执行这些类型的更新。</span><span class="sxs-lookup"><span data-stu-id="9e534-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="9e534-109">有关详细信息, 请参阅[office 365 终结点类别和 Office 365 IP 地址和 URL web 服务](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。</span><span class="sxs-lookup"><span data-stu-id="9e534-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
