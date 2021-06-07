---
title: Microsoft 365 导入服务中的驱动器传送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721667"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="9fb53-102">Microsoft 365 导入服务中的驱动器传送</span><span class="sxs-lookup"><span data-stu-id="9fb53-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="9fb53-103">使用驱动器传送，将 PSTS 复制到硬盘，然后将硬盘发运到 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="9fb53-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="9fb53-104">请按照以下步骤开始操作:</span><span class="sxs-lookup"><span data-stu-id="9fb53-104">To start the job:</span></span>

1. <span data-ttu-id="9fb53-105">在 Microsoft 365 合规中心的“**信息治理”** 下，选择“**导入**”。</span><span class="sxs-lookup"><span data-stu-id="9fb53-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="9fb53-106">选择“**选择导入作业类型**”，然后选择“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="9fb53-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="9fb53-107">若要查看此导入选项的步骤，请选择“**将硬盘传送到我们其中的一个物理位置**”。</span><span class="sxs-lookup"><span data-stu-id="9fb53-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="9fb53-108">以下是几点注意事项:</span><span class="sxs-lookup"><span data-stu-id="9fb53-108">Here are some things to remember:</span></span>

- <span data-ttu-id="9fb53-109">必须分配有 Exchange Online 中的邮箱导入导出角色，才能将 PST 文件导入到 Microsoft 365 邮箱。</span><span class="sxs-lookup"><span data-stu-id="9fb53-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="9fb53-110">PST 超过 20GB 可能会影响性能。</span><span class="sxs-lookup"><span data-stu-id="9fb53-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="9fb53-111">仅支持将 2.5 英寸固态硬盘 (SSD) 或 2.5 英寸或 3.5 英寸 SATA II/III 内部硬盘。</span><span class="sxs-lookup"><span data-stu-id="9fb53-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="9fb53-112">包含 PST 文件的硬盘必须使用 BitLocker 进行加密。</span><span class="sxs-lookup"><span data-stu-id="9fb53-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="9fb53-113">使用驱动器传送将 PST 文件导入到 Microsoft 365 邮箱的成本为每 GB 数据 2 美元。</span><span class="sxs-lookup"><span data-stu-id="9fb53-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="9fb53-114">有关使用驱动器传送方法导入 PST 的其他信息，请参阅[使用驱动器传送导入组织的 PST 文件](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)。</span><span class="sxs-lookup"><span data-stu-id="9fb53-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>