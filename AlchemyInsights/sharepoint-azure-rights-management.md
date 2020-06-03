---
title: 在 SharePoint 或 OneDrive 中限制访问权限
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 77f9938fe40d9f693ccce1dac3581625ed7e424a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509554"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="3e166-102">对 SharePoint 文件的 IRM 保护</span><span class="sxs-lookup"><span data-stu-id="3e166-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="3e166-103">在 SharePoint Online 中，IRM 保护应用于列表和库级别的文件。</span><span class="sxs-lookup"><span data-stu-id="3e166-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="3e166-104">您的组织可以使用 IRM 保护之前，必须先设置权限管理。</span><span class="sxs-lookup"><span data-stu-id="3e166-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="3e166-105">IRM 依赖 azure 权限管理服务（来自 Azure 信息保护）来加密和分配使用限制。</span><span class="sxs-lookup"><span data-stu-id="3e166-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="3e166-106">一些 Microsoft 365 订阅包括 Azure 权限管理，但并非全部。</span><span class="sxs-lookup"><span data-stu-id="3e166-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="3e166-107">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="3e166-107">To learn more, see:</span></span>

- <span data-ttu-id="3e166-108">[Office 应用程序和服务如何支持 Azure 权限管理](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)。</span><span class="sxs-lookup"><span data-stu-id="3e166-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="3e166-109">[在 SharePoint 管理中心中设置信息权限管理（IRM）](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="3e166-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="3e166-110">[IRM-启用 SharePoint 文档库和列表](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)。</span><span class="sxs-lookup"><span data-stu-id="3e166-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="3e166-111">[Office 中的信息权限管理](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)。</span><span class="sxs-lookup"><span data-stu-id="3e166-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="3e166-112">[Exchange Online 中的信息权限管理](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="3e166-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


