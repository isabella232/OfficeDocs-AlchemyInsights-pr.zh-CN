---
title: 向通讯组添加外部用户？
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: a5def36fbb662037851158722db60494f00ce850
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2019
ms.locfileid: "34895195"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="1f514-102">向通讯组添加外部用户？</span><span class="sxs-lookup"><span data-stu-id="1f514-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="1f514-103">向通讯组添加外部联系人 (DG) 的过程分两步:</span><span class="sxs-lookup"><span data-stu-id="1f514-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="1f514-104">为外部用户创建邮件联系人:</span><span class="sxs-lookup"><span data-stu-id="1f514-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="1f514-105">单击[此处](https://admin.microsoft.com/adminportal/home#/Contact)导航到管理门户中的联系人编辑页。</span><span class="sxs-lookup"><span data-stu-id="1f514-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="1f514-106">单击 "**添加联系人**"。</span><span class="sxs-lookup"><span data-stu-id="1f514-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="1f514-107">键入您的联系人的信息, 然后单击 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="1f514-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="1f514-108">将邮件联系人添加到你的 DG:</span><span class="sxs-lookup"><span data-stu-id="1f514-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="1f514-109">单击[此处](https://admin.microsoft.com/adminportal/home#/groups)导航到 "组" 页面。</span><span class="sxs-lookup"><span data-stu-id="1f514-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="1f514-110">找到要向其添加外部用户的 DG, 然后单击该 DG 以打开 "编辑" 对话框。</span><span class="sxs-lookup"><span data-stu-id="1f514-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="1f514-111">单击 "**成员**" 列表中的 "**编辑**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="1f514-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="1f514-112">单击 "**添加成员**"。</span><span class="sxs-lookup"><span data-stu-id="1f514-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="1f514-113">选择您在上一步中创建的邮件联系人, 然后单击 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="1f514-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="1f514-114">即使在执行这些步骤之后, 外部用户也无法向 DG 发送电子邮件或不接收来自该 DG 的电子邮件, 也可以将该 DG 标记为只允许来自内部用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1f514-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="1f514-115">您可以按照[此处](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)的说明检查此配置并将其修复</span><span class="sxs-lookup"><span data-stu-id="1f514-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="1f514-116">**注意:** 如果您的组的类型是 "Office 365 组" 而不是 "通讯组", 则不适用这些说明。</span><span class="sxs-lookup"><span data-stu-id="1f514-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="1f514-117">如果是这种情况, 则可以将外部用户直接添加到 Outlook 或 Web 上的 Outlook 中的组。</span><span class="sxs-lookup"><span data-stu-id="1f514-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="1f514-118">有关 O365 组来宾的详细说明, 以及有关添加外部来宾的说明, 请参阅[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。</span><span class="sxs-lookup"><span data-stu-id="1f514-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  