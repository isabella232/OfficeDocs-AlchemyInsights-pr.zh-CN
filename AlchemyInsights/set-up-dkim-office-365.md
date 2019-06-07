---
title: Office 365 中的安装 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764879"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="83d6e-102">Office 365 中的安装 DKIM</span><span class="sxs-lookup"><span data-stu-id="83d6e-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="83d6e-103">在 Office 365 中为自定义域配置 DKIM 的完整说明如下[](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)所示。</span><span class="sxs-lookup"><span data-stu-id="83d6e-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="83d6e-104">对于**每个**自定义域, 您需要在您的域的 DNS 托管服务 (通常为域注册机构) 中创建**两个**DKIM CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="83d6e-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="83d6e-105">例如, contoso.com 和 fourthcoffee.com 需要四个 DKIM CNAME 记录: 两个用于 contoso.com, 两个用于 fourthcoffee.com。</span><span class="sxs-lookup"><span data-stu-id="83d6e-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="83d6e-106">**每个**自定义域的 DKIM CNAME 记录使用以下格式:</span><span class="sxs-lookup"><span data-stu-id="83d6e-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="83d6e-107">**主机名**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="83d6e-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="83d6e-108">**指向 "地址" 或 "值**":`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="83d6e-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="83d6e-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="83d6e-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="83d6e-110">**主机名**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="83d6e-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="83d6e-111">**指向 "地址" 或 "值**":`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="83d6e-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="83d6e-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="83d6e-112">**TTL**: 3600</span></span>

   <span data-ttu-id="83d6e-113">\<DomainGUID\>是自定义域的自定义 MX `.mail.protection.outlook.com`记录 (例如, `contoso-com`域 contoso.com) 的左侧文本。</span><span class="sxs-lookup"><span data-stu-id="83d6e-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="83d6e-114">\<InitialDomain\>是注册 Office 365 时使用的域 (例如, contoso.onmicrosoft.com)。</span><span class="sxs-lookup"><span data-stu-id="83d6e-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="83d6e-115">为自定义域创建 CNAME 记录后, 请完成以下说明:</span><span class="sxs-lookup"><span data-stu-id="83d6e-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="83d6e-116">a.</span><span class="sxs-lookup"><span data-stu-id="83d6e-116">a.</span></span> <span data-ttu-id="83d6e-117">使用您的 工作或学校帐户[登录到 Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)。</span><span class="sxs-lookup"><span data-stu-id="83d6e-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="83d6e-118">b.</span><span class="sxs-lookup"><span data-stu-id="83d6e-118">b.</span></span> <span data-ttu-id="83d6e-119">选择左上角的应用启动器图标，然后选择“**管理员**”。</span><span class="sxs-lookup"><span data-stu-id="83d6e-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="83d6e-120">c.</span><span class="sxs-lookup"><span data-stu-id="83d6e-120">c.</span></span> <span data-ttu-id="83d6e-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="83d6e-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="83d6e-122">d.</span><span class="sxs-lookup"><span data-stu-id="83d6e-122">d.</span></span> <span data-ttu-id="83d6e-123">转到**保护** > **DKIM**。</span><span class="sxs-lookup"><span data-stu-id="83d6e-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="83d6e-124">e.</span><span class="sxs-lookup"><span data-stu-id="83d6e-124">e.</span></span> <span data-ttu-id="83d6e-125">选择域, 然后选择 " \*\*\*\* 为**此域使用 DKIM 签名启用签名邮件**"。</span><span class="sxs-lookup"><span data-stu-id="83d6e-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="83d6e-126">为每个自定义域重复执行这一步。</span><span class="sxs-lookup"><span data-stu-id="83d6e-126">Repeat this step for each custom domain.</span></span>
