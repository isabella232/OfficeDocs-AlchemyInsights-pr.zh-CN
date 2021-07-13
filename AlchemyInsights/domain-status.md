---
title: 域状态 - 未选择任何服务
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389168"
---
# <a name="domain-status---no-services-selected"></a><span data-ttu-id="e8d0e-102">域状态 - 未选择任何服务</span><span class="sxs-lookup"><span data-stu-id="e8d0e-102">Domain Status - No services selected</span></span>

<span data-ttu-id="e8d0e-103">**未选择** 任何服务意味着你尚未选择任何 Microsoft 365 服务（如 Exchange Online、Skype for Business 或 Intune）和移动设备管理Microsoft 365用于自定义域。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-103">**No services selected** means you haven’t selected any Microsoft 365 services such as Exchange Online, Skype for Business or Intune, and Mobile Device Management for Microsoft 365 to use with your custom domain.</span></span> <span data-ttu-id="e8d0e-104">如果在本地将 Exchange 混合 (Exchange与 Exchange Online) 或外部垃圾邮件筛选一Exchange，Microsoft 服务，可以忽略此邮件。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-104">If you're using Exchange Hybrid (Exchange on-premises with Exchange Online) or external spam filtering with Exchange and no other Microsoft services, you can ignore this message.</span></span> <span data-ttu-id="e8d0e-105">域运行状况状态仅适用于直接连接到服务的域。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-105">Domain health status is available only for domains connected directly to the service.</span></span>

<span data-ttu-id="e8d0e-106">若要为域选择服务：</span><span class="sxs-lookup"><span data-stu-id="e8d0e-106">To select services for your domain:</span></span>

1. <span data-ttu-id="e8d0e-107">From **设置**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home)， check the box next to the domain with the status message **No services selected**.</span><span class="sxs-lookup"><span data-stu-id="e8d0e-107">From **Settings** > [**Domains**](https://admin.microsoft.com/Adminportal/Home), check the box next to the domain with the status message **No services selected**.</span></span>
1. <span data-ttu-id="e8d0e-108">选择 **"管理 DNS"** 以启动域设置向导。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-108">Select **Manage DNS** to start the Domain Setup Wizard.</span></span>
    - <span data-ttu-id="e8d0e-109">如果选择" **添加自己的 DNS 记录"，** 请确保在系统提示时选择服务。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-109">If you choose **Add your own DNS records**, be sure to select a service when prompted.</span></span> <span data-ttu-id="e8d0e-110">高级选项 下可能提供了 **更多服务**。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-110">More services could be available under **Advanced Options**.</span></span>
    - <span data-ttu-id="e8d0e-111">如果选择"**允许 Microsoft 添加 DNS** 记录"或"更多选项""为我设置联机服务"，将自动建议和选择  >  所有可用服务。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-111">If you choose **Let Microsoft add your DNS records** or **More options** > **Setup my online services for me** all available services are suggested and selected automatically.</span></span>
1. <span data-ttu-id="e8d0e-112">继续执行向导以完成 DNS 设置和服务选择。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-112">Continue through the wizard to complete DNS setup and your service choices.</span></span>
 
<span data-ttu-id="e8d0e-113">有关设置域的其他帮助，请参阅添加 [DNS 记录以连接域](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="e8d0e-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

