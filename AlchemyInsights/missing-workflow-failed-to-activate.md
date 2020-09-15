---
title: 无法激活缺少的工作流
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667076"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8e044-102">无法激活缺少的工作流</span><span class="sxs-lookup"><span data-stu-id="8e044-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8e044-103">在 Microsoft SharePoint 网站集中，无法将全局可重用工作流 (如 "审批-SharePoint 2010" ) 添加到列表或库中。</span><span class="sxs-lookup"><span data-stu-id="8e044-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8e044-104">若要解决此问题，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="8e044-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8e044-105">在 SharePoint Designer 2013 中打开网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="8e044-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8e044-106">在 " **网站对象**" 下，选择 " **工作流**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8e044-107">在 "**工作流**" 功能区的 "**新建**" 部分，选择 "**可重用工作流**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8e044-108">在 " **创建可重用工作流** " 表单中，输入名称 \* \* *Repair2010* \* \*。</span><span class="sxs-lookup"><span data-stu-id="8e044-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8e044-109">对于 " **平台类型**"，单击 " **SharePoint 2010 工作流**"，然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="8e044-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8e044-110">在 "**工作流**" 功能区的 "**保存**" 部分，选择 "**发布**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8e044-111">在 "**工作流**" 功能区的 "**管理**" 部分，选择 "**全局发布**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8e044-112">在出现的确认对话框中，选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="8e044-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8e044-113">在 web 浏览器中，找到网站集的根网站，然后访问 " **网站设置**" \> **网站集功能**。</span><span class="sxs-lookup"><span data-stu-id="8e044-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8e044-114">然后，切换 **工作流** 功能：</span><span class="sxs-lookup"><span data-stu-id="8e044-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8e044-115">·如果功能已  *激活*  ，请单击 " **停用"，** 然后单击 " **激活**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8e044-116">·如果  *禁用*  该功能，请单击 " **激活**"。</span><span class="sxs-lookup"><span data-stu-id="8e044-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8e044-117">有关详细信息，请参阅以下 [文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="8e044-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

