---
title: 无法添加2010审批工作流
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558607"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="94153-102">无法添加2010审批工作流</span><span class="sxs-lookup"><span data-stu-id="94153-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="94153-103">在 Microsoft SharePoint 网站集中, 无法将全局可重用工作流 (如 "审批-SharePoint 2010") 添加到列表或库。</span><span class="sxs-lookup"><span data-stu-id="94153-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="94153-104">若要解决此问题, 请按照下列步骤操作:</span><span class="sxs-lookup"><span data-stu-id="94153-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="94153-105">在 SharePoint Designer 2013 中打开网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="94153-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="94153-106">在 "**网站对象**" 下, 选择 "**工作流**"。</span><span class="sxs-lookup"><span data-stu-id="94153-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="94153-107">在 "**工作流**" 功能区的 "**新建**" 部分, 选择 "**可重用工作流**"。</span><span class="sxs-lookup"><span data-stu-id="94153-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="94153-108">在 "**创建可重用工作流**" 表单中, 输入名称 \* \* *Repair2010* \* \*。</span><span class="sxs-lookup"><span data-stu-id="94153-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="94153-109">对于 "**平台类型**", 单击 " **SharePoint 2010 工作流**", 然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="94153-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="94153-110">在 "**工作流**" 功能区的 "**保存**" 部分, 选择 "**发布**"。</span><span class="sxs-lookup"><span data-stu-id="94153-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="94153-111">在 "**工作流**" 功能区的 "**管理**" 部分, 选择 "**全局发布**"。</span><span class="sxs-lookup"><span data-stu-id="94153-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="94153-112">在出现的确认对话框中, 选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="94153-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="94153-113">在 web 浏览器中, 找到网站集的根网站, 然后访问 "**网站设置** \> "**网站集功能**。</span><span class="sxs-lookup"><span data-stu-id="94153-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="94153-114">切换**工作流**功能:</span><span class="sxs-lookup"><span data-stu-id="94153-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="94153-115">·如果功能已*激活*, 请单击 "**停用",** 然后单击 "**激活**"。</span><span class="sxs-lookup"><span data-stu-id="94153-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="94153-116">·如果*禁用*该功能, 请单击 "**激活**"。</span><span class="sxs-lookup"><span data-stu-id="94153-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="94153-117">有关详细信息, 请参阅以下[文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="94153-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

