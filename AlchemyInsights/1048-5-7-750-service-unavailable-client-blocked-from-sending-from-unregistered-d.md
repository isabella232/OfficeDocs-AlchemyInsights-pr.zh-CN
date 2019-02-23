---
title: 1048 5.7.750 服务不可用。阻止从未注册的域发送的客户端
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.openlocfilehash: 356bb008da3b08c320e6afde84c310629cc3be81
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/22/2019
ms.locfileid: "30208971"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="5008d-103">阻止从未注册域发送的5.7.750 客户端</span><span class="sxs-lookup"><span data-stu-id="5008d-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="5008d-104">当从未在 Office 365 中预配的域 (添加为接受域并经过验证) 中发送大量邮件时, 将发生此错误。</span><span class="sxs-lookup"><span data-stu-id="5008d-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="5008d-105">若要避免此错误, 可以使用基于证书的邮件流连接器 (其中证书的域是已设置的域), 也可以设置所有发送域。</span><span class="sxs-lookup"><span data-stu-id="5008d-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

