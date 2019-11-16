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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769329"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>如果以编程方式更改字段，则不会发生 OnChange 事件

如果使用属性以编程方式更改字段，则不会发生*OnChange*事件 *。*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)方法。 如果您希望在设置值之后运行*OnChange*事件的事件处理程序，必须在代码中使用*formContext 属性* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)方法。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
