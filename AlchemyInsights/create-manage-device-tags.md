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
ms.openlocfilehash: c06ed00d7cf4bcb23fdcee12f446953918075728
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325639"
---
# <a name="create-and-manage-device-tags-or-groups"></a>创建和管理设备标签或组

在设备上添加标记，创建逻辑组等同。 设备标记支持网络适当映射，可附加不同的标记以捕获上下文，并启用在事件过程中创建动态列表。 标记可用于设备列表视图中的筛选器或组设备。 有关设备分组详细信息，请参阅 [创建和管理设备标记](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)。

可以在设备上添加标记，操作者：

- 使用门户

- 设置注册表项值
 
**注意：** 将标记添加到设备的时间及其在设备列表和设备页面中的可用性之间可能存在延迟。

若要使用 API 添加设备标记，请参阅 [添加或删除设备标记 API](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)。

## <a name="add-and-manage-device-tags-using-the-portal"></a>使用门户添加和管理设备标记

1. 选择要用于管理标签的设备。 可以从以下任一视图选择或搜索设备：

    - **安全操作仪表板** 具有活动警报部分的顶部设备中选择设备名称。
    - **警报队列** - 从警报队列中选择设备图标旁边的设备名称。
    - **设备列表** - 从设备列表中选择设备名称。
    - **搜索框** - 从下拉菜单中选择设备，然后输入设备名称。

    还可通过文件和 IP 视图访问警报页面。

1. 从响应操作行中选择 **管理标签**。

1. 键入以查找或创建标签。

标记将添加到设备视图，并反映在设备列表视图中。 然后可使用"标记"筛选器查看设备的相关列表。

有关详细信息，请参阅 [创建和管理设备标签](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)。