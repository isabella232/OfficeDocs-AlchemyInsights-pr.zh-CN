---
title: 1048 5.7.750 服务不可用。 阻止从未注册的域发送的客户端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: b94fcc697bb7ac065cef57f3e3eb0b515c3094a0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352843"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="5188f-103">阻止从未注册域发送的5.7.750 客户端</span><span class="sxs-lookup"><span data-stu-id="5188f-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="5188f-104">当从未在 Office 365 中预配的域 (添加为接受域并经过验证) 中发送大量邮件时, 将发生此错误。</span><span class="sxs-lookup"><span data-stu-id="5188f-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="5188f-105">若要避免此错误, 可以使用基于证书的邮件流连接器 (其中证书的域是已设置的域), 也可以设置所有发送域。</span><span class="sxs-lookup"><span data-stu-id="5188f-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
