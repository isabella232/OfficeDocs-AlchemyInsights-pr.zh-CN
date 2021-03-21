---
title: 从 Yammer 导入和导出
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897542"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="7a36b-102">从 Yammer 导入和导出</span><span class="sxs-lookup"><span data-stu-id="7a36b-102">Import and export from Yammer</span></span>

<span data-ttu-id="7a36b-103">**导入**</span><span class="sxs-lookup"><span data-stu-id="7a36b-103">**Import**</span></span>

<span data-ttu-id="7a36b-104">根据你的 Yammer 网络是否处于[适用于 Microsoft 365 的本机模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)，用户导入选项会有所不同。</span><span class="sxs-lookup"><span data-stu-id="7a36b-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="7a36b-105">**非本机模式**：可以使用组设置中的“[从地址簿添加](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294)”（最多 100 个用户）将用户导入组，或在“网络管理”中使用“[批量更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)”将用户导入网络。</span><span class="sxs-lookup"><span data-stu-id="7a36b-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="7a36b-106">**本机模式**：组成员资格和网络成员资格操作应从 [Microsoft 365 管理门户网站](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD 门户网站](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)或使用其他 Azure AD 选项执行。</span><span class="sxs-lookup"><span data-stu-id="7a36b-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="7a36b-107">本机模式下的网络不可再访问批量更新和其他旧版功能。</span><span class="sxs-lookup"><span data-stu-id="7a36b-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7a36b-108">即使在另一个网络中使用了数据导出功能，Yammer 也不支持从“网络管理”中导入内容。</span><span class="sxs-lookup"><span data-stu-id="7a36b-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="7a36b-109">可通过合作伙伴解决方案或 Yammer REST API 重新发布内容。</span><span class="sxs-lookup"><span data-stu-id="7a36b-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="7a36b-110">**导出**</span><span class="sxs-lookup"><span data-stu-id="7a36b-110">**Export**</span></span>

<span data-ttu-id="7a36b-111">[在“网络管理”中导出网络数据](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)允许从 Yammer 网络导出内容，包括消息和文件。</span><span class="sxs-lookup"><span data-stu-id="7a36b-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="7a36b-112">附件可能很大，并且会导致需要花费大量时间才能完成导出。</span><span class="sxs-lookup"><span data-stu-id="7a36b-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="7a36b-113">我们建议使用[数据导出 API](https://developer.yammer.com/docs/data-export-api) 按区块导出每天或每周的活动网络。</span><span class="sxs-lookup"><span data-stu-id="7a36b-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="7a36b-114">Microsoft 支持不会为此提供自定义脚本。</span><span class="sxs-lookup"><span data-stu-id="7a36b-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="7a36b-115">存在单独的 [GDPR 导出](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)，用于导出单个用户的内容。</span><span class="sxs-lookup"><span data-stu-id="7a36b-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>