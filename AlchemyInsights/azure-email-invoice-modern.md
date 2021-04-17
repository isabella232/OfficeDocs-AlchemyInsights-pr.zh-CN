---
title: 新式 Azure 电子邮件发票
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820816"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="a6fd2-102">Azure 中的电子邮件发票</span><span class="sxs-lookup"><span data-stu-id="a6fd2-102">Email invoicing in Azure</span></span>

<span data-ttu-id="a6fd2-103">必须在帐单配置文件或其帐单帐户中拥有所有者或参与者角色，才能更新其电子邮件发票首选项。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="a6fd2-104">选择加入后，在帐单配置文件中拥有所有者、参与者、读者和发票管理员角色的所有用户都将在电子邮件中获取发票。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="a6fd2-105">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a6fd2-106">搜索“**成本管理 + 帐单**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="a6fd2-107">从左侧选择“**发票**”，然后从页面顶部选择“**使用电子邮件发送发票**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="a6fd2-108">如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“**选择加入**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="a6fd2-109">选择 **“更新”**。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-109">Select **Update**.</span></span>
6. <span data-ttu-id="a6fd2-110">如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“**选择加入**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="a6fd2-111">对于 MCA 或 MPA 帐单配置文件，你可通过向其分配发票管理员角色，授予其查看、下载和支付发票的权限。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="a6fd2-112">如果你选择要在电子邮件中获取发票，用户也会在电子邮件中获取发票。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="a6fd2-113">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a6fd2-114">搜索“**成本管理 + 帐单**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="a6fd2-115">从左侧选择“**计费对象信息**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="a6fd2-116">从“帐单配置文件”列表中，选择要为其分配发票管理员角色的帐单配置文件。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="a6fd2-117">从左侧选择 “**访问控制（IAM）**” ，然后选择从页面顶部选择“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="a6fd2-118">在“角色”下拉列表中，选择“**发票管理员**”。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="a6fd2-119">输入要向其授予访问权限的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="a6fd2-120">选择“**保存**”以分配角色。</span><span class="sxs-lookup"><span data-stu-id="a6fd2-120">Select **Save** to assign the role.</span></span>
