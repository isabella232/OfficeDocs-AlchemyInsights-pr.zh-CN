---
title: 在 Intune 中自动清理陈旧设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715011"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>在 Intune 中自动清理陈旧设备

Intune 允许管理员配置 90 和 270 天之间的时间间隔，之后将从服务中删除陈旧设备。 此设置是组织范围的，激活后将立即生效。 在超过设置的时间段内未签入 Intune 服务器的任何设备都将被永久删除。

**注意** 只有 MDM 设备对象才有资格执行此清除操作。 仅排除了 EAS 设备对象。

有关根据设备清理设置及其“状态”何时可以删除设备的其他信息：

设置：**上次签入日期后删除设备：是（指定天数内的某些值 (N)）**

- 根据设置中配置的值 (N)，Intune 服务会在上次成功签入的指定天数内删除设备。

设置：**上次签入日期后删除设备：否**

- 设备证书过期且未续订 180 天后，将删除该设备。

**注意** 在两种情况下，必须在 Intune 中成功登记设备。 第一次使用 Intune 服务签入设备的过程中将发生登记。

如果设备向 Intune 成功注册但未在 Intune 中登记，则设备将在注册后 270 天内删除。 （头 90 天将设备标记为已吊销，接下来的 180 天删除记录。）

Intune 控制台中当前没有任何机制可用于确定任何给定设备的设备认证到期日期。