---
title: 故障排除错误404，找不到文件
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750081"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="91717-102">故障排除错误404，找不到文件</span><span class="sxs-lookup"><span data-stu-id="91717-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="91717-103">当用户尝试访问 SharePoint 或 OneDrive 中的网站或文件时，收到错误404。</span><span class="sxs-lookup"><span data-stu-id="91717-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="91717-104">这通常是由于网站或文件或组被重命名、移动或删除所致。</span><span class="sxs-lookup"><span data-stu-id="91717-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="91717-105">例如：用户将在尝试访问根网站集时遇到404错误，并且已将其删除。</span><span class="sxs-lookup"><span data-stu-id="91717-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="91717-106">若要解决已重命名、移动或删除的网站的错误404，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="91717-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="91717-107">对于经典管理中心中存在的经典网站，请参阅 [还原已删除的网站集](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)。</span><span class="sxs-lookup"><span data-stu-id="91717-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="91717-108">对于新式网站 (与新 SharePoint 管理中心中存在的通信、组连接或其他网站) ，请参阅在 [新 sharepoint 管理中心中查看和还原已删除的网站](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)。</span><span class="sxs-lookup"><span data-stu-id="91717-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="91717-109">若要解决文件 (或其他已重命名、移动或删除的项目) 的错误404，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="91717-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="91717-110">转到 SharePoint 或 OneDrive 网站，并从网站内容中查看回收站。</span><span class="sxs-lookup"><span data-stu-id="91717-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="91717-111">请参阅 [在 SharePoint 网站的回收站中还原项目](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)。</span><span class="sxs-lookup"><span data-stu-id="91717-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="91717-112">如果仍无法找到该项目，则可以搜索审核日志（如果已启用日志记录）。若要了解，请 [在 Microsoft 365 Security & 合规性中心中搜索审核日志](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。</span><span class="sxs-lookup"><span data-stu-id="91717-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
