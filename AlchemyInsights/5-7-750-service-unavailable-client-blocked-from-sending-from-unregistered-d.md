---
title: 1048 5.7.750 服务不可用。 阻止从未注册的域发送的客户端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664232"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="cc06a-103">5.7.750 客户端无法通过未注册的域发送邮件</span><span class="sxs-lookup"><span data-stu-id="cc06a-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="cc06a-104">如果从未在租户中预配的域发送大量邮件， (添加为接受的域并经过验证) ，则会发生此错误。</span><span class="sxs-lookup"><span data-stu-id="cc06a-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="cc06a-105">若要避免此错误，可以使用基于证书的邮件流连接器（其中证书的域是已设置的域），也可以设置所有发送域。</span><span class="sxs-lookup"><span data-stu-id="cc06a-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
