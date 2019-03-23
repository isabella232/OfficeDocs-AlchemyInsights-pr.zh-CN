---
title: 1049反垃圾邮件4.5.3 收件人太多 (AS780090)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1049
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: 363214d75c255d2f493e6a771749d2c2817042f0
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30780447"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="77ed6-102">4.5.3 收件人过多 (AS780090)</span><span class="sxs-lookup"><span data-stu-id="77ed6-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="77ed6-103">当来自源 ip 地址的电子邮件流量超出了源 ip 地址的信誉 (或缺少信誉) 限制时, 将发生此错误。</span><span class="sxs-lookup"><span data-stu-id="77ed6-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>
  
<span data-ttu-id="77ed6-104">阻止来自源 IP 地址的电子邮件将在一小时内过期。</span><span class="sxs-lookup"><span data-stu-id="77ed6-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="77ed6-105">如果源 IP 地址是属于您的本地电子邮件服务器, 请验证邮件流连接器的配置。</span><span class="sxs-lookup"><span data-stu-id="77ed6-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="77ed6-106">如果此行为持续时间超过一小时, 请联系支持人员请求提供源 IP 地址的例外。</span><span class="sxs-lookup"><span data-stu-id="77ed6-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
  
