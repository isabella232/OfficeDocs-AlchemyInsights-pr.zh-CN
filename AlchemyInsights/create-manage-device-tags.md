---
title: 创建和管理设备标签或组
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
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721678"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="90b1a-102">创建和管理设备标签或组</span><span class="sxs-lookup"><span data-stu-id="90b1a-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="90b1a-103">在设备上添加标记，创建逻辑组等同。</span><span class="sxs-lookup"><span data-stu-id="90b1a-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="90b1a-104">设备标记支持网络适当映射，可附加不同的标记以捕获上下文，并启用在事件过程中创建动态列表。</span><span class="sxs-lookup"><span data-stu-id="90b1a-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="90b1a-105">标记可用于设备列表视图中的筛选器或组设备。</span><span class="sxs-lookup"><span data-stu-id="90b1a-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="90b1a-106">有关设备分组详细信息，请参阅 [创建和管理设备标记](/microsoft-365/security/defender-endpoint/machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="90b1a-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="90b1a-107">可以在设备上添加标记，操作者：</span><span class="sxs-lookup"><span data-stu-id="90b1a-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="90b1a-108">使用门户</span><span class="sxs-lookup"><span data-stu-id="90b1a-108">Using the portal</span></span>

- <span data-ttu-id="90b1a-109">设置注册表项值</span><span class="sxs-lookup"><span data-stu-id="90b1a-109">Setting a registry key value</span></span>
 
<span data-ttu-id="90b1a-110">**注意：** 将标记添加到设备的时间及其在设备列表和设备页面中的可用性之间可能存在延迟。</span><span class="sxs-lookup"><span data-stu-id="90b1a-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="90b1a-111">若要使用 API 添加设备标记，请参阅 [添加或删除设备标记 API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="90b1a-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="90b1a-112">使用门户添加和管理设备标记</span><span class="sxs-lookup"><span data-stu-id="90b1a-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="90b1a-113">选择要用于管理标签的设备。</span><span class="sxs-lookup"><span data-stu-id="90b1a-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="90b1a-114">可以从以下任一视图选择或搜索设备：</span><span class="sxs-lookup"><span data-stu-id="90b1a-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="90b1a-115">**安全操作仪表板** 具有活动警报部分的顶部设备中选择设备名称。</span><span class="sxs-lookup"><span data-stu-id="90b1a-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="90b1a-116">**警报队列** - 从警报队列中选择设备图标旁边的设备名称。</span><span class="sxs-lookup"><span data-stu-id="90b1a-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="90b1a-117">**设备列表** - 从设备列表中选择设备名称。</span><span class="sxs-lookup"><span data-stu-id="90b1a-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="90b1a-118">**搜索框** - 从下拉菜单中选择设备，然后输入设备名称。</span><span class="sxs-lookup"><span data-stu-id="90b1a-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="90b1a-119">还可通过文件和 IP 视图访问警报页面。</span><span class="sxs-lookup"><span data-stu-id="90b1a-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="90b1a-120">从响应操作行中选择 **管理标签**。</span><span class="sxs-lookup"><span data-stu-id="90b1a-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="90b1a-121">键入以查找或创建标签。</span><span class="sxs-lookup"><span data-stu-id="90b1a-121">Type to find or create tags.</span></span>

<span data-ttu-id="90b1a-122">标记将添加到设备视图，并反映在设备列表视图中。</span><span class="sxs-lookup"><span data-stu-id="90b1a-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="90b1a-123">然后可使用"标记"筛选器查看设备的相关列表。</span><span class="sxs-lookup"><span data-stu-id="90b1a-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="90b1a-124">有关详细信息，请参阅 [创建和管理设备标签](/microsoft-365/security/defender-endpoint/machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="90b1a-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>