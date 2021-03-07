---
title: 配置 Workday 到 AD 的用户设置进入隔离状态
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430714"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>配置 Workday 到 AD 的用户设置进入隔离状态

**配置 Workday 到 AD 的用户设置进入隔离状态，AD 中未创建任何用户**

配置 Workday 到 AD 的用户设置作业已进入隔离状态，审核日志显示导出失败事件，错误信息 **错误：OperationsError-SvcErr：发生操作错误。没有为目录服务配置任何高级参考。因此，目录服务无法向此域林外部的对象发出引用**。 如果未正确设置 Active Directory 容器 OU，或者用于 **parentDistingishedName** 的表达式映射存在问题，则通常会显示这个错误。

检查 **"新用户** 默认 OU参数是否有错别字。 确保 AD 中已存在指定的 OU。 如果在属性映射中 **使用 parentDistingishedName** ，请确保它始终计算到 AD 域中的已知容器。 检查审核日志中的导出事件，可查看生成的值。

有关配置 workday 以实现自动设置的更多细节，请参阅 [教程：为自动用户设置配置 Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。

