---
title: 将网站或列表另存为模板
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770518"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="27ba4-102">将网站或列表另存为模板</span><span class="sxs-lookup"><span data-stu-id="27ba4-102">Save site or list as a template</span></span>

<span data-ttu-id="27ba4-103">SharePoint 网站模板是围绕特定的业务需要设计的预制定义。</span><span class="sxs-lookup"><span data-stu-id="27ba4-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="27ba4-104">有关详细信息, 请参阅[使用模板创建不同种类的 SharePoint 网站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。</span><span class="sxs-lookup"><span data-stu-id="27ba4-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="27ba4-105">下面是有关在 SharePoint Online 中将网站或列表保存为模板的一些常见问题/解决方案。</span><span class="sxs-lookup"><span data-stu-id="27ba4-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="27ba4-106">"**保存网站/列表模板" 按钮不可用或缺失**。</span><span class="sxs-lookup"><span data-stu-id="27ba4-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="27ba4-107">管理员将需要允许自定义脚本启用模板功能。</span><span class="sxs-lookup"><span data-stu-id="27ba4-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="27ba4-108">有关详细步骤、示例和注意事项, 请参阅[Allow or 预防自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="27ba4-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="27ba4-109">"将网站另存为模板" 命令不受支持, 并且可能会在使用 SharePoint Server 发布基础结构的网站上出现问题。</span><span class="sxs-lookup"><span data-stu-id="27ba4-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="27ba4-110">**网站模板无法创建或无法正常工作**</span><span class="sxs-lookup"><span data-stu-id="27ba4-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="27ba4-111">模板可能缺少[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx), 无法激活。</span><span class="sxs-lookup"><span data-stu-id="27ba4-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="27ba4-112">如果在当前网站集中无法激活该功能, 则不能使用网站模板创建网站。</span><span class="sxs-lookup"><span data-stu-id="27ba4-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="27ba4-113">检查以查看是否有任何列表或库超出了5000个项目的[列表视图限制阈值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), 因为这可能会阻止创建网站模板。</span><span class="sxs-lookup"><span data-stu-id="27ba4-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="27ba4-114">网站可能使用过多的资源, 因此网站模板超过了 50 mb 的限制。</span><span class="sxs-lookup"><span data-stu-id="27ba4-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="27ba4-115">显示使用查阅列的列表中的数据时出现问题。</span><span class="sxs-lookup"><span data-stu-id="27ba4-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="27ba4-116">有关详细信息, 请参阅[模板生成的列表不会在 SharePoint Online 中显示正确的查找列表中的数据](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。</span><span class="sxs-lookup"><span data-stu-id="27ba4-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="27ba4-117">有关常见问题和解决方案的更多详细信息, 请参阅[创建和使用网站模板](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="27ba4-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

