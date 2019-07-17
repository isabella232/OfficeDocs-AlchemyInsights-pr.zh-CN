---
title: Dynamics 365 Forms 业务规则-表单无法触发业务规则
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747013"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>如果以编程方式更改字段, 则不会发生 OnChange 事件

如果使用属性以编程方式更改字段, 则不会发生*OnChange*事件 *。*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)方法。 如果您希望在设置值之后运行*OnChange*事件的事件处理程序, 则必须使用*formContext 属性。* 代码中的[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)方法。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
