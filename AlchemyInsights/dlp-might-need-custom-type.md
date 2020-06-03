---
title: DLP 可能需要自定义类型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507504"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1f72f-102">DLP 可能需要自定义类型</span><span class="sxs-lookup"><span data-stu-id="1f72f-102">DLP might need a custom type</span></span>

<span data-ttu-id="1f72f-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="1f72f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1f72f-104">**DLP 可能需要自定义信息类型**</span><span class="sxs-lookup"><span data-stu-id="1f72f-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="1f72f-105">使用数据丢失防护（DLP）策略，可以识别和保护组织中的敏感数据。</span><span class="sxs-lookup"><span data-stu-id="1f72f-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1f72f-106">在某些情况下，您可能需要创建自己的**自定义**敏感信息类型来保护组织的数据。</span><span class="sxs-lookup"><span data-stu-id="1f72f-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1f72f-107">例如，您的组织可能需要以特定于您的组织的某种格式标识和保护员工 Id 或其他数据。如果是这样，请参阅以下文章以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="1f72f-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="1f72f-108">**自定义内置敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="1f72f-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1f72f-109">如果内置的敏感信息类型只满足几次调整，就能满足您的需求，则可以[自定义内置的敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="1f72f-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1f72f-110">例如，您可以添加或删除关键字，或者添加或删除支持的证据，如日期或地址。</span><span class="sxs-lookup"><span data-stu-id="1f72f-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1f72f-111">**创建自定义敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="1f72f-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1f72f-112">但是，如果您需要完全标识和保护不同类型的敏感信息，则可以在安全 & 合规性中心的 UI 中[创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="1f72f-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="1f72f-113">**使用安全与合规中心 PowerShell 创建自定义敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="1f72f-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1f72f-114">最后，如果 UI 不提供您所需的所有选项，则可以[在 Security & 合规性中心 PowerShell 中创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="1f72f-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1f72f-115">从 XML 文件开始，可以使用每个可用的选项。</span><span class="sxs-lookup"><span data-stu-id="1f72f-115">By starting with an XML file, you can use every option available.</span></span>
