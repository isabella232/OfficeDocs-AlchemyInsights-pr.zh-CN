---
title: 传输服务 - 将所有 RDFE 服务移动到其他订阅
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681452"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="c331b-102">传输服务 - 将所有 RDFE 服务移动到其他订阅</span><span class="sxs-lookup"><span data-stu-id="c331b-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="c331b-103">**移动资源**</span><span class="sxs-lookup"><span data-stu-id="c331b-103">**Move resources**</span></span>

<span data-ttu-id="c331b-104">可以使用 Azure 门户、Azure PowerShell、Azure CLI 或 REST API 将 Azure 资源移动到同一订阅下的另一个 Azure 订阅或资源组，以移动资源。</span><span class="sxs-lookup"><span data-stu-id="c331b-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="c331b-105">在移动资源之前，请参阅：</span><span class="sxs-lookup"><span data-stu-id="c331b-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="c331b-106">移动资源前检查表</span><span class="sxs-lookup"><span data-stu-id="c331b-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="c331b-107">可以移动的服务</span><span class="sxs-lookup"><span data-stu-id="c331b-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c331b-108">如何验证移动</span><span class="sxs-lookup"><span data-stu-id="c331b-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="c331b-109">服务移动指南</span><span class="sxs-lookup"><span data-stu-id="c331b-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="c331b-110">若要将现有资源移动到其他资源组或订阅，可以使用：</span><span class="sxs-lookup"><span data-stu-id="c331b-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="c331b-111">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="c331b-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="c331b-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c331b-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="c331b-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c331b-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="c331b-114">REST API</span><span class="sxs-lookup"><span data-stu-id="c331b-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="c331b-115">教程： [将 Azure 资源移动到其他资源组或订阅](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="c331b-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="c331b-116">**Azure 资源管理器错误疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c331b-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="c331b-117">请参阅以下文章，了解一些常见的 Azure 部署错误，并接收解决这些问题的信息。</span><span class="sxs-lookup"><span data-stu-id="c331b-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="c331b-118">如果找不到部署错误的错误代码，请参阅["查找错误代码"。](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)</span><span class="sxs-lookup"><span data-stu-id="c331b-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="c331b-119">解决部署错误</span><span class="sxs-lookup"><span data-stu-id="c331b-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="c331b-120">将 Azure 资源移动到新资源组或订阅疑难解答</span><span class="sxs-lookup"><span data-stu-id="c331b-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="c331b-121">请注意，如果你想要升级 Azure 订阅，例如从免费切换到即付即用，你将需要转换你的订阅。</span><span class="sxs-lookup"><span data-stu-id="c331b-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="c331b-122">若要升级免费试用版，请参阅将免费试用版或 Microsoft Imagine Azure 订阅升级到即付 [即用](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)。</span><span class="sxs-lookup"><span data-stu-id="c331b-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="c331b-123">若要更改即付即用帐户，请参阅将 Azure 即付即用订阅更改为 [其他优惠](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)。</span><span class="sxs-lookup"><span data-stu-id="c331b-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="c331b-124">**若要向 Azure Active Directory 租户添加或关联 Azure 订阅：**</span><span class="sxs-lookup"><span data-stu-id="c331b-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="c331b-125">从 Azure 门户的"订阅"页面登录并选择 [想要使用的订阅](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)。</span><span class="sxs-lookup"><span data-stu-id="c331b-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="c331b-126">选择 **"更改目录"。**</span><span class="sxs-lookup"><span data-stu-id="c331b-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="c331b-127">查看出现的任何警告，然后选择"更改 **"。**</span><span class="sxs-lookup"><span data-stu-id="c331b-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="c331b-128">订阅的目录已更改，你将收到一条成功消息。</span><span class="sxs-lookup"><span data-stu-id="c331b-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="c331b-129">使用 *目录切换* 程序转到新目录。</span><span class="sxs-lookup"><span data-stu-id="c331b-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="c331b-130">可能需要 10 分钟才能正确显示所有内容。</span><span class="sxs-lookup"><span data-stu-id="c331b-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="c331b-131">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="c331b-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="c331b-132">转移 Azure 订阅的所有权</span><span class="sxs-lookup"><span data-stu-id="c331b-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="c331b-133">将资源移动到新资源组或订阅</span><span class="sxs-lookup"><span data-stu-id="c331b-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="c331b-134">使用 Azure 门户管理资源</span><span class="sxs-lookup"><span data-stu-id="c331b-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
