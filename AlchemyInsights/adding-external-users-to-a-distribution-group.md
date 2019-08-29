---
title: 向通讯组添加外部用户
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660782"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="c0ef2-102">将外部用户添加到通讯组</span><span class="sxs-lookup"><span data-stu-id="c0ef2-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="c0ef2-103">向通讯组添加外部联系人 (DG) 的过程分为两个步骤:</span><span class="sxs-lookup"><span data-stu-id="c0ef2-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="c0ef2-104">为外部用户创建邮件联系人:</span><span class="sxs-lookup"><span data-stu-id="c0ef2-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="c0ef2-105">在管理中心中, 转到 "**用户** > [联系人](https://admin.microsoft.com/adminportal/home#/Contact)" 页。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="c0ef2-106">选择 "**添加联系人**"。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="c0ef2-107">键入您的联系人的信息, 然后选择 "**添加**"。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="c0ef2-108">将邮件联系人添加到你的 DG:</span><span class="sxs-lookup"><span data-stu-id="c0ef2-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="c0ef2-109">在 "管理中心" 中, 转到 "**组** > [组](https://admin.microsoft.com/adminportal/home#/groups)" 页面。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="c0ef2-110">找到要向其添加外部用户的 DG, 然后选择该 DG 以打开 "编辑" 对话框。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="c0ef2-111">在 "**成员**" 选项卡上, 选择 "**查看所有和管理成员**"。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="c0ef2-112">选择 "**添加成员**"。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="c0ef2-113">选择您在上一步中创建的邮件联系人, 然后选择 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="c0ef2-114">如果执行这些步骤后, 你的外部用户无法向 DG 发送电子邮件或不接收来自该 DG 的电子邮件, 则可能会将此 DG 标记为仅允许来自内部用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="c0ef2-115">您可以查看此配置并按照[此处](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)的说明进行修复。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="c0ef2-116">**注意:** 如果您的组的类型是 "Office 365 组" 而不是 "通讯组", 则不适用这些说明。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="c0ef2-117">如果是这种情况, 则可以将外部用户直接添加到 Outlook 中的组。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="c0ef2-118">有关 Office 365 组来宾的详细信息, 以及有关如何添加外部来宾的说明, 请参阅[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c0ef2-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  