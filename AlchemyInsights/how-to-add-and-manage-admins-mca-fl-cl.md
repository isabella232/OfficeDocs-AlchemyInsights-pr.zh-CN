---
title: 如何添加和管理管理员 - MCA FL/CL
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49683946"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="03040-102">如何添加和管理管理员 - MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="03040-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="03040-103">若要管理 MCA (Microsoft 客户协议) 帐户，可以使用具有所需访问权限级别的不同角色。</span><span class="sxs-lookup"><span data-stu-id="03040-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="03040-104">这些角色是内置 Azure 服务角色之外，可帮助你控制资源。</span><span class="sxs-lookup"><span data-stu-id="03040-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="03040-105">**若要在 Azure 门户中添加计费角色：**</span><span class="sxs-lookup"><span data-stu-id="03040-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="03040-106">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="03040-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="03040-107">搜索 *成本管理 + 计费*。</span><span class="sxs-lookup"><span data-stu-id="03040-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="03040-108">Select Access control (IAM) 作用域，如计费帐户、 帐单配置文件或发票部分，你要授予访问权限。</span><span class="sxs-lookup"><span data-stu-id="03040-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="03040-109">IAM (访问控制) 列出了分配给该作用域的每个角色的用户和组。</span><span class="sxs-lookup"><span data-stu-id="03040-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="03040-110">若要向用户授予访问权限 **，请从** 页面顶部选择"添加"。</span><span class="sxs-lookup"><span data-stu-id="03040-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="03040-111">在 *"角色* "下拉列表中，选择一个角色。</span><span class="sxs-lookup"><span data-stu-id="03040-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="03040-112">输入要授予其访问权限的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="03040-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="03040-113">选择 **"保存** "以分配角色。</span><span class="sxs-lookup"><span data-stu-id="03040-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="03040-114">若要删除用户的访问权限，请选择具有要删除角色分配的用户。</span><span class="sxs-lookup"><span data-stu-id="03040-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="03040-115">选择 **"删除"。**</span><span class="sxs-lookup"><span data-stu-id="03040-115">Select **Remove**.</span></span>

<span data-ttu-id="03040-116">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="03040-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="03040-117">计费角色定义</span><span class="sxs-lookup"><span data-stu-id="03040-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="03040-118">计费帐户角色和任务</span><span class="sxs-lookup"><span data-stu-id="03040-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="03040-119">开始使用 MCA 计费帐户</span><span class="sxs-lookup"><span data-stu-id="03040-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="03040-120">检查对 Microsoft 客户协议的访问权限</span><span class="sxs-lookup"><span data-stu-id="03040-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
