---
title: 无法设置或查看 AllowSelfServicePurchase 策略
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091666"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="121d2-102">无法设置或查看 AllowSelfServicePurchase 策略</span><span class="sxs-lookup"><span data-stu-id="121d2-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="121d2-103">在尝试设置或查看 AllowSelfServicePurchase 策略时，您会收到以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="121d2-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="121d2-104">*HandleError：无法检索带有 PolicyId "AllowSelfServicePurchase" 的产品策略，错误-基础连接已关闭：发送时发生意外错误。*</span><span class="sxs-lookup"><span data-stu-id="121d2-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="121d2-105">这可能是由于较旧版本的传输层安全性（TLS）造成的。</span><span class="sxs-lookup"><span data-stu-id="121d2-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="121d2-106">若要连接 MSCommerce 服务，您需要使用 TLS 1.2 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="121d2-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="121d2-107">尝试执行以下步骤，将 TLS 协议启用/设置为1.2、验证和重试。</span><span class="sxs-lookup"><span data-stu-id="121d2-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="121d2-108">在 PowerShell 命令提示符（PS C：\) ）中，输入以下命令，将 TLS 协议设置为版本1.2：</span><span class="sxs-lookup"><span data-stu-id="121d2-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="121d2-109">\[ServicePointManager]：： SecurityProtocol = \[SecurityProtocolType]：： Tls12</span><span class="sxs-lookup"><span data-stu-id="121d2-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="121d2-110">使用以下命令验证所使用的 TLS 协议：</span><span class="sxs-lookup"><span data-stu-id="121d2-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="121d2-111">\[ServicePointManager]：： SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="121d2-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="121d2-112">根据需要，重试 Get 或 Update 命令。</span><span class="sxs-lookup"><span data-stu-id="121d2-112">Retry the Get or Update commands as needed.</span></span>

