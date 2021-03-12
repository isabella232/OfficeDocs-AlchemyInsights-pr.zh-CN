---
title: 还原已删除的文件或文件夹
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707512"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="bca2d-102">还原已删除的文件或文件夹</span><span class="sxs-lookup"><span data-stu-id="bca2d-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="bca2d-103">除实际删除外，SharePoint Online 会将所有内容的备份再保留 14 天。</span><span class="sxs-lookup"><span data-stu-id="bca2d-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="bca2d-104">如果无法通过回收站或文件还原还原内容，管理员可以在 14 天窗口中随时联系 Microsoft 支持部门请求还原。</span><span class="sxs-lookup"><span data-stu-id="bca2d-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="bca2d-105">自备份还原仅能为网站集或子站点完成，不适用于特定文件、列表或库。</span><span class="sxs-lookup"><span data-stu-id="bca2d-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="bca2d-106">当您从 Sharepoint 中删除项目或网站时，不会立即将其删除。</span><span class="sxs-lookup"><span data-stu-id="bca2d-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="bca2d-107">删除的项目会在回收站保留一段时间。</span><span class="sxs-lookup"><span data-stu-id="bca2d-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="bca2d-108">在此期间，可以将已删除的项目还原到原始位置。</span><span class="sxs-lookup"><span data-stu-id="bca2d-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="bca2d-109">有关详细信息，请访问以下链接。</span><span class="sxs-lookup"><span data-stu-id="bca2d-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="bca2d-110">[还原 SharePoint 网站的回收站中的项目](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)。</span><span class="sxs-lookup"><span data-stu-id="bca2d-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="bca2d-111">在 OneDrive 中还原已删除的文件或文件夹</span><span class="sxs-lookup"><span data-stu-id="bca2d-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="bca2d-112">还原已删除的网站集 (包括组、通信和其他网站) </span><span class="sxs-lookup"><span data-stu-id="bca2d-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="bca2d-113">还原已删除的 OneDrive 网站</span><span class="sxs-lookup"><span data-stu-id="bca2d-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="bca2d-114">对于批量回收站操作，管理员可以考虑使用[Sharepoint Online PNP。](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="bca2d-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="bca2d-115">**文件还原功能**</span><span class="sxs-lookup"><span data-stu-id="bca2d-115">**Files Restore feature**</span></span>

<span data-ttu-id="bca2d-116">如果大量 OneDrive 或 SharePoint 文件被恶意软件删除、覆盖、损坏或感染，可以使用文件还原功能将整个 OneDrive 或 SharePoint 库还原到以前的时间。</span><span class="sxs-lookup"><span data-stu-id="bca2d-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="bca2d-117">还原 OneDrive 库</span><span class="sxs-lookup"><span data-stu-id="bca2d-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="bca2d-118">还原文档库</span><span class="sxs-lookup"><span data-stu-id="bca2d-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

