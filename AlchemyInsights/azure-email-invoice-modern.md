---
title: 新式 Azure 电子邮件发票
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840570"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="6c738-102">Azure 中的电子邮件发票</span><span class="sxs-lookup"><span data-stu-id="6c738-102">Email invoicing in Azure</span></span>

<span data-ttu-id="6c738-103">必须在帐单配置文件或其帐单帐户中拥有所有者或参与者角色，才能更新其电子邮件发票首选项。</span><span class="sxs-lookup"><span data-stu-id="6c738-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="6c738-104">选择加入后，在帐单配置文件中拥有所有者、参与者、读者和发票管理员角色的所有用户都将在电子邮件中获取发票。</span><span class="sxs-lookup"><span data-stu-id="6c738-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="6c738-105">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="6c738-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6c738-106">搜索“ **成本管理 + 帐单** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6c738-107">从左侧选择“ **发票** ”，然后从页面顶部选择“ **使用电子邮件发送发票** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="6c738-108">如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“ **选择加入** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="6c738-109">选择 **“更新”** 。</span><span class="sxs-lookup"><span data-stu-id="6c738-109">Select **Update**.</span></span>
6. <span data-ttu-id="6c738-110">如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“ **选择加入** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="6c738-111">对于 MCA 或 MPA 帐单配置文件，你可通过向其分配发票管理员角色，授予其查看、下载和支付发票的权限。</span><span class="sxs-lookup"><span data-stu-id="6c738-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="6c738-112">如果你选择要在电子邮件中获取发票，用户也会在电子邮件中获取发票。</span><span class="sxs-lookup"><span data-stu-id="6c738-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="6c738-113">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="6c738-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6c738-114">搜索“ **成本管理 + 帐单** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6c738-115">从左侧选择“ **帐单配置文件** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="6c738-116">从“帐单配置文件”列表中，选择要为其分配发票管理员角色的帐单配置文件。</span><span class="sxs-lookup"><span data-stu-id="6c738-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="6c738-117">从左侧选择 “ **访问控制（IAM）** ” ，然后选择从页面顶部选择“ **添加** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="6c738-118">在“角色”下拉列表中，选择“ **发票管理员** ”。</span><span class="sxs-lookup"><span data-stu-id="6c738-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="6c738-119">输入要向其授予访问权限的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6c738-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="6c738-120">选择“ **保存** ”以分配角色。</span><span class="sxs-lookup"><span data-stu-id="6c738-120">Select **Save** to assign the role.</span></span>
