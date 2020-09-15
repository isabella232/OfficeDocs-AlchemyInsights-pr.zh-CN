---
title: AIP：策略未按预期运行
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663179"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="cc7b0-102">AIP：策略未按预期运行</span><span class="sxs-lookup"><span data-stu-id="cc7b0-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="cc7b0-103">Azure 信息保护：策略未按预期运行，有关各种策略问题的建议准则，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="cc7b0-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="cc7b0-104">如果你在视觉标记方面遇到问题，请查看[应用视觉标记时](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="cc7b0-105">如果使用自动标记时遇到问题，请查看[如何为 Azure 信息保护配置自动分类和推荐分类条件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)和[敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="cc7b0-106">如果你在本机/配置文件保护方面遇到问题，请查看[文件 API 配置](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="cc7b0-107">检查是否使用了配置不正确的作用域内策略：[如何通过使用作用域内策略为特定用户配置 Azure 信息保护策略](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="cc7b0-108">如果附加标记文档时，Outlook 无法使用自动标记，验证是否未按下列说明定义 DRMEncryptProperty：[针对安全的 IRM 注册表设置](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="cc7b0-109">如果仍遇到问题，请收集 Azure 信息保护客户端日志，并将导出的日志附加到此票证。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="cc7b0-110">在 Outlook 中打开 Office 文档或新建电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="cc7b0-111">单击“**保护/敏感度**” > “**帮助和反馈**。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="cc7b0-112">单击“**导出日志**”。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="cc7b0-113">将日志保存到选定位置，并将其附加到此服务请求中。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="cc7b0-114">其他资源：</span><span class="sxs-lookup"><span data-stu-id="cc7b0-114">Additional resources:</span></span>

- [<span data-ttu-id="cc7b0-115">如何为 Azure 信息保护配置用于视觉标记的标签</span><span class="sxs-lookup"><span data-stu-id="cc7b0-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="cc7b0-116">查阅 Azure 信息保护文档</span><span class="sxs-lookup"><span data-stu-id="cc7b0-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="cc7b0-117">在 Microsoft 365 应用中使用敏感度标签</span><span class="sxs-lookup"><span data-stu-id="cc7b0-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

