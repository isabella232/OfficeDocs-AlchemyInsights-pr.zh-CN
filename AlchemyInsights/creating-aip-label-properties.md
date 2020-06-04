---
title: 创建 AIP 标签策略
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542082"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="90387-102">创建 AIP 标签策略</span><span class="sxs-lookup"><span data-stu-id="90387-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="90387-103">Azure 信息保护（AIP）标签可与组织通常创建和存储的完整数据范围（从最小的个人数据分类到高度机密数据的最大分类）一起使用。</span><span class="sxs-lookup"><span data-stu-id="90387-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="90387-104">Azure 信息保护策略适用于 Azure 信息保护（AIP）经典客户端，而不是[AIP 统一标记客户端](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)。</span><span class="sxs-lookup"><span data-stu-id="90387-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="90387-105">您可以在 AIP 策略中配置多个元素，包括如下选项：</span><span class="sxs-lookup"><span data-stu-id="90387-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="90387-106">选项，该选项将允许管理员或用户对文档和电子邮件进行分类和保护（可选）</span><span class="sxs-lookup"><span data-stu-id="90387-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="90387-107">在用户保存文档和发送电子邮件时强制进行分类的选项</span><span class="sxs-lookup"><span data-stu-id="90387-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="90387-108">根据电子邮件的附件自动为其添加标签的选项。</span><span class="sxs-lookup"><span data-stu-id="90387-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="90387-109">用于控制是否在 Office 应用程序中显示信息保护栏的选项</span><span class="sxs-lookup"><span data-stu-id="90387-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="90387-110">有关 Azure 信息保护策略的其他选项和信息，请参阅： [Azure 信息保护策略概述](https://docs.microsoft.com/azure/information-protection/overview-policy)。</span><span class="sxs-lookup"><span data-stu-id="90387-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="90387-111">有关 AIP 策略的其他有用资源，请参阅：</span><span class="sxs-lookup"><span data-stu-id="90387-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="90387-112">教程：配置 Azure 信息保护策略设置并创建新标签</span><span class="sxs-lookup"><span data-stu-id="90387-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="90387-113">配置 Azure 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="90387-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="90387-114">创建和配置敏感度标签及其策略</span><span class="sxs-lookup"><span data-stu-id="90387-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="90387-115">使用 Azure 信息保护的常见方案的操作方法指南</span><span class="sxs-lookup"><span data-stu-id="90387-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="90387-116">查看 Azure 信息保护文档</span><span class="sxs-lookup"><span data-stu-id="90387-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="90387-117">Azure 信息保护的要求</span><span class="sxs-lookup"><span data-stu-id="90387-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="90387-118">Azure 信息保护的快速入门教程</span><span class="sxs-lookup"><span data-stu-id="90387-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="90387-119">下载 Azure 信息保护客户端</span><span class="sxs-lookup"><span data-stu-id="90387-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)