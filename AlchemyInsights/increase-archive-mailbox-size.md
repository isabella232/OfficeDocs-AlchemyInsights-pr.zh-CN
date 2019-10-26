---
title: 305增加存档邮箱大小
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36661790"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="43093-102">增加存档邮箱大小</span><span class="sxs-lookup"><span data-stu-id="43093-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="43093-103">Office 365 根据分配给用户帐户的许可证[限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)存档邮箱的大小。</span><span class="sxs-lookup"><span data-stu-id="43093-103">Office 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="43093-104">当存档邮箱达到其允许大小的90% 时，用户将收到电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="43093-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="43093-105">当存档邮箱达到其大小限制时，用户将无法将更多项目移至存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="43093-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="43093-106">一旦达到大小限制，Office 365 将不会增加存档邮箱的大小。</span><span class="sxs-lookup"><span data-stu-id="43093-106">Office 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="43093-107">相反，用户可以执行以下操作来释放存档邮箱中的空间：</span><span class="sxs-lookup"><span data-stu-id="43093-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="43093-108">使用 Outlook 将项目导出到 .pst 文件。</span><span class="sxs-lookup"><span data-stu-id="43093-108">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="43093-109">删除存档邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="43093-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="43093-110">Office 365 提供了 Office 365 企业版 E3 和 E5 许可证的**无限制存档**。</span><span class="sxs-lookup"><span data-stu-id="43093-110">Office 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="43093-111">管理员必须先启用此功能，存档邮箱才能达到其最大大小。</span><span class="sxs-lookup"><span data-stu-id="43093-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="43093-112">启用无限期存档时，最长可能需要30天，才能将可用空间添加到存档邮箱中。</span><span class="sxs-lookup"><span data-stu-id="43093-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="43093-113">因此，我们建议管理员验证存档邮箱中的可用空间，以便用户可以在扩展时继续使用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="43093-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="43093-114">有关详细信息，请参阅[office 365 中的无限制存档概述](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)和[在 Office 365 中启用无限制存档](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)。</span><span class="sxs-lookup"><span data-stu-id="43093-114">For more information, see [Overview of unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) and [Enable unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="43093-115">有关从 Outlook 访问存档邮箱的详细信息，请参阅[访问自动扩展存档中的项目的 Outlook 要求](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)。</span><span class="sxs-lookup"><span data-stu-id="43093-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="43093-116">若要配置自动将项目移动到存档邮箱的保留策略，请参阅为[Office 365 组织中的邮箱设置存档和删除策略](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="43093-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Office 365 organization](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="43093-117">**注意**： Exchange 2010 上的主邮箱不支持自动扩展存档。</span><span class="sxs-lookup"><span data-stu-id="43093-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
