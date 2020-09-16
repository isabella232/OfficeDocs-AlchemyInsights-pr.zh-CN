---
title: 创建 AIP 标签策略
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732165"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="f61f3-102">创建 AIP 标签策略</span><span class="sxs-lookup"><span data-stu-id="f61f3-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="f61f3-103">Azure 信息保护 (AIP) 标签可用于组织通常创建和存储的完整数据范围，从最小的个人数据分类到高度机密数据的最大分类。</span><span class="sxs-lookup"><span data-stu-id="f61f3-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="f61f3-104">Azure 信息保护策略适用于 Azure 信息保护 (AIP) 经典客户端，而不是  [AIP 统一标记客户端](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)。</span><span class="sxs-lookup"><span data-stu-id="f61f3-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="f61f3-105">您可以在 AIP 策略中配置多个元素，包括如下选项：</span><span class="sxs-lookup"><span data-stu-id="f61f3-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="f61f3-106">可供管理员或用户对其进行分类和保护 (可选) 文档和电子邮件的标签的选项</span><span class="sxs-lookup"><span data-stu-id="f61f3-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="f61f3-107">在用户保存文档和发送电子邮件时强制进行分类的选项</span><span class="sxs-lookup"><span data-stu-id="f61f3-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="f61f3-108">根据电子邮件的附件自动为其添加标签的选项。</span><span class="sxs-lookup"><span data-stu-id="f61f3-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="f61f3-109">用于控制是否在 Office 应用程序中显示信息保护栏的选项</span><span class="sxs-lookup"><span data-stu-id="f61f3-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="f61f3-110">有关 Azure 信息保护策略的其他选项和信息，请参阅： [Azure 信息保护策略概述](https://docs.microsoft.com/azure/information-protection/overview-policy)。</span><span class="sxs-lookup"><span data-stu-id="f61f3-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="f61f3-111">有关 AIP 策略的其他有用资源，请参阅：</span><span class="sxs-lookup"><span data-stu-id="f61f3-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="f61f3-112">教程：配置 Azure 信息保护策略设置和创建新标签</span><span class="sxs-lookup"><span data-stu-id="f61f3-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="f61f3-113">配置 Azure 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="f61f3-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="f61f3-114">创建和配置敏感度标签及其策略</span><span class="sxs-lookup"><span data-stu-id="f61f3-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="f61f3-115">有关使用 Azure 信息保护常见方案的操作指南</span><span class="sxs-lookup"><span data-stu-id="f61f3-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="f61f3-116">查阅 Azure 信息保护文档</span><span class="sxs-lookup"><span data-stu-id="f61f3-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="f61f3-117">Azure 信息保护要求</span><span class="sxs-lookup"><span data-stu-id="f61f3-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="f61f3-118">Azure 信息保护快速入门教程</span><span class="sxs-lookup"><span data-stu-id="f61f3-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="f61f3-119">下载 Azure 信息保护客户端</span><span class="sxs-lookup"><span data-stu-id="f61f3-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)