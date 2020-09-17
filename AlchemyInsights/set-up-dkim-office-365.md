---
title: 安装 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808697"
---
# <a name="setup-dkim"></a><span data-ttu-id="31144-102">安装 DKIM</span><span class="sxs-lookup"><span data-stu-id="31144-102">Setup DKIM</span></span>

<span data-ttu-id="31144-103">在 Microsoft 365 中为自定义域配置 DKIM 的完整[说明如下所示。](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="31144-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="31144-104">对于 **每个** 自定义域，您需要在您的域的 DNS 托管服务 (中创建 **两个** DKIM CNAME 记录。通常，域注册器) 。</span><span class="sxs-lookup"><span data-stu-id="31144-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="31144-105">例如，contoso.com 和 fourthcoffee.com 需要四个 DKIM CNAME 记录：两个用于 contoso.com，两个用于 fourthcoffee.com。</span><span class="sxs-lookup"><span data-stu-id="31144-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="31144-106">**每个**自定义域的 DKIM CNAME 记录使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="31144-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="31144-107">**主机名**： `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="31144-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="31144-108">**指向 "地址" 或 "值**"： `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="31144-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="31144-109">**TTL**：3600</span><span class="sxs-lookup"><span data-stu-id="31144-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="31144-110">**主机名**： `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="31144-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="31144-111">**指向 "地址" 或 "值**"： `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="31144-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="31144-112">**TTL**：3600</span><span class="sxs-lookup"><span data-stu-id="31144-112">**TTL**: 3600</span></span>

   <span data-ttu-id="31144-113">\<DomainGUID\> 是左侧的自定义域的 `.mail.protection.outlook.com` 自定义 MX 记录中的文本 (例如， `contoso-com` 对于 domain contoso.com) 。</span><span class="sxs-lookup"><span data-stu-id="31144-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="31144-114">\<InitialDomain\> 是注册 Microsoft 365 时使用的域 (例如，contoso.onmicrosoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="31144-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="31144-115">为自定义域创建 CNAME 记录后，请完成以下说明：</span><span class="sxs-lookup"><span data-stu-id="31144-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="31144-116">a.</span><span class="sxs-lookup"><span data-stu-id="31144-116">a.</span></span> <span data-ttu-id="31144-117">使用你的工作或学校帐户[登录到 Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 。</span><span class="sxs-lookup"><span data-stu-id="31144-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="31144-118">b.</span><span class="sxs-lookup"><span data-stu-id="31144-118">b.</span></span> <span data-ttu-id="31144-119">选择左上角的应用启动器图标，然后选择“**管理员**”。</span><span class="sxs-lookup"><span data-stu-id="31144-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="31144-120">c.</span><span class="sxs-lookup"><span data-stu-id="31144-120">c.</span></span> <span data-ttu-id="31144-121">在左下侧导航中，展开“管理”并选择“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="31144-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="31144-122">d.</span><span class="sxs-lookup"><span data-stu-id="31144-122">d.</span></span> <span data-ttu-id="31144-123">转到**保护**  >  **DKIM**。</span><span class="sxs-lookup"><span data-stu-id="31144-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="31144-124">e.</span><span class="sxs-lookup"><span data-stu-id="31144-124">e.</span></span> <span data-ttu-id="31144-125">选择域，然后选择 " **Enable**为**此域使用 DKIM 签名启用签名邮件**"。</span><span class="sxs-lookup"><span data-stu-id="31144-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="31144-126">为每个自定义域重复执行这一步。</span><span class="sxs-lookup"><span data-stu-id="31144-126">Repeat this step for each custom domain.</span></span>
