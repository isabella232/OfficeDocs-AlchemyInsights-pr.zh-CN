---
title: 1048 5.7.750 服务不可用。 阻止从未注册的域发送的客户端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676703"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="87e2e-103">5.7.750 客户端无法通过未注册的域发送邮件</span><span class="sxs-lookup"><span data-stu-id="87e2e-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="87e2e-104">当从未在租户中预配的域发送大量邮件（添加为接受的域并经过验证）时，将发生此错误。</span><span class="sxs-lookup"><span data-stu-id="87e2e-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="87e2e-105">若要避免此错误，可以使用基于证书的邮件流连接器（其中证书的域是已设置的域），也可以设置所有发送域。</span><span class="sxs-lookup"><span data-stu-id="87e2e-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
