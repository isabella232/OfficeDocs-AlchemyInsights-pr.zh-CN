---
title: 修复了 DKIM 记录格式的常见问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500708"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="b15d4-102">修复了 DKIM 记录格式的常见问题</span><span class="sxs-lookup"><span data-stu-id="b15d4-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="b15d4-103">大多数 DKIM 设置问题与不正确的 DNS 记录相关。</span><span class="sxs-lookup"><span data-stu-id="b15d4-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="b15d4-104">若要修复 DKIM 设置问题，请验证 DKIM CNAME 记录 (TXT 记录是否) 格式正确。 </span><span class="sxs-lookup"><span data-stu-id="b15d4-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="b15d4-105">有关详细信息，请参阅在 [Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)中手动设置 DKIM 需要执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="b15d4-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="b15d4-106">如果需要有关 DNS 记录的一般帮助，请参阅在任何 DNS 托管提供商处为 [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)创建 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="b15d4-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="b15d4-107">在域的 DNS 托管服务处创建或更新 DKIM DNS 记录后，需要等待 DNS 记录传播。</span><span class="sxs-lookup"><span data-stu-id="b15d4-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
