---
title: 错误代码 AADSTS50011 故障排除
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901600"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="5ac24-102">错误代码 AADSTS50011 故障排除</span><span class="sxs-lookup"><span data-stu-id="5ac24-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="5ac24-103">如果要解决 AADSTS50011 错误，请执行以下推荐步骤。</span><span class="sxs-lookup"><span data-stu-id="5ac24-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="5ac24-104">**AADSTS50011**: InvalidReplyTo - 答复地址丢失、配置错误或与为应用配置的回复地址不匹配。</span><span class="sxs-lookup"><span data-stu-id="5ac24-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="5ac24-105">作为解决方法，请确保将此缺失的回复地址添加到 Azure Active Directory (AD) 应用中，或让有权限在 AD 中管理应用程序的人来执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5ac24-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="5ac24-106">有关详细信息，请参阅错误[AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch)的疑难解答文章。</span><span class="sxs-lookup"><span data-stu-id="5ac24-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>