---
title: 使用 AIP 客户端自动分类行为异常
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 8c79ab50e7ddbda0cf61eb9a95279f6c42cc515c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581185"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="f6d73-102">使用 AIP 客户端自动分类行为异常</span><span class="sxs-lookup"><span data-stu-id="f6d73-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="f6d73-103">自动分类行为异常时，使用下列推荐的指南：</span><span class="sxs-lookup"><span data-stu-id="f6d73-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="f6d73-104">如果使用自动标记时遇到问题，请参阅[如何为 Azure 信息保护配置自动分类和推荐分类条件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)和[敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。</span><span class="sxs-lookup"><span data-stu-id="f6d73-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="f6d73-105">检查是否使用了配置不正确的作用域内策略：[如何通过使用作用域内策略为特定用户配置 Azure 信息保护策略](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)。</span><span class="sxs-lookup"><span data-stu-id="f6d73-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="f6d73-106">如果附加标记文档时，Outlook 无法使用自动标记，验证未按下列说明定义 `DRMEncryptProperty`：[针对安全的 IRM 注册表设置](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。</span><span class="sxs-lookup"><span data-stu-id="f6d73-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="f6d73-107">如果将[内置信息类型](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)用于 Azure 信息保护策略，请验证内容是否与预期格式匹配。</span><span class="sxs-lookup"><span data-stu-id="f6d73-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="f6d73-108">验证标签是否已针对**自动**或**推荐**进行了相应配置。</span><span class="sxs-lookup"><span data-stu-id="f6d73-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="f6d73-109">（**自动**标记可用于所有 Microsoft 365 应用程序，而**推荐**可用于除 Outlook 之外的所有 Microsoft 365 应用程序。）</span><span class="sxs-lookup"><span data-stu-id="f6d73-109">(**Automatic** labeling is available for all Microsoft 365 apps, whereas **Recommended** is available for all Microsoft 365 apps except for Outlook.)</span></span>
6. <span data-ttu-id="f6d73-110">不可对之前已手动标记或者之前已自动标记有更高级分类的文档和电子邮件使用自动分类。</span><span class="sxs-lookup"><span data-stu-id="f6d73-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="f6d73-111">有关详细信息，请参阅：[如何应用自动标签或建议标签](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="f6d73-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="f6d73-112">如果仍遇到问题，请收集 Azure 信息保护客户端日志，并将导出的日志附加到支持票证。</span><span class="sxs-lookup"><span data-stu-id="f6d73-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="f6d73-113">导出 Azure 信息保护日志：</span><span class="sxs-lookup"><span data-stu-id="f6d73-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="f6d73-114">在 Outlook 中打开 Office 文档或新建电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f6d73-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="f6d73-115">单击“**保护/敏感度**” > “**帮助和反馈**。</span><span class="sxs-lookup"><span data-stu-id="f6d73-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="f6d73-116">单击“**导出日志**”。</span><span class="sxs-lookup"><span data-stu-id="f6d73-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="f6d73-117">将日志保存到选定位置，并将其附加到服务请求中。</span><span class="sxs-lookup"><span data-stu-id="f6d73-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="f6d73-118">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="f6d73-118">For additional information, see:</span></span>

- [<span data-ttu-id="f6d73-119">如何为 Azure 信息保护配置自动分类和推荐分类条件</span><span class="sxs-lookup"><span data-stu-id="f6d73-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="f6d73-120">有关使用 Azure 信息保护常见方案的操作指南</span><span class="sxs-lookup"><span data-stu-id="f6d73-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="f6d73-121">查阅 Azure 信息保护文档</span><span class="sxs-lookup"><span data-stu-id="f6d73-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f6d73-122">查阅 Azure 信息保护订阅和功能</span><span class="sxs-lookup"><span data-stu-id="f6d73-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="f6d73-123">Azure 信息保护要求</span><span class="sxs-lookup"><span data-stu-id="f6d73-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="f6d73-124">Azure 信息保护快速入门教程</span><span class="sxs-lookup"><span data-stu-id="f6d73-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="f6d73-125">下载 Azure 信息保护客户端</span><span class="sxs-lookup"><span data-stu-id="f6d73-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
