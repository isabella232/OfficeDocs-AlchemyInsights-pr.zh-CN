---
title: 管理中心Exchange保留策略无法工作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074922"
---
# <a name="retention-policies-in-exchange-admin-center"></a>管理中心Exchange策略

如果您希望我们针对下面提到的设置运行自动检查，请选择此页面顶部的"后退"按钮"<"，然后输入与保留策略有问题的用户的电子邮件地址。

如果您在管理中心中遇到保留策略Exchange管理中心不适用于邮箱或未移动到存档邮箱的项目，请检查以下内容：

**根本原因：**

- **托管文件夹** 助理尚未处理用户的邮箱。 托管文件夹助理每七天尝试处理一次基于云的组织内每个邮箱。

  **解决方案：** 运行托管文件夹助理。

- 已在邮箱上 **启用** **RetentionHold。** 如果邮箱已置于 RetentionHold 中，则在此期间将不会处理邮箱的保留策略。

  **解决方案：** 根据需要检查"保留保留"设置和更新的状态。 有关详细信息，请参阅邮箱 [保留保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
 
**注意：** 如果邮箱小于 10 MB，托管文件夹助理不会自动处理邮箱。
 
有关管理中心中保留策略Exchange，请参阅：

- [保留标记和保留策略](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [将保留策略应用于邮箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 或 [添加或删除保留标记](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [如何识别为邮箱设置的保留类型](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
