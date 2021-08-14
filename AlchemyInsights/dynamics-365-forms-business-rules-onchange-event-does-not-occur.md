---
title: Dynamics 365 Forms Business Rules - 不为窗体触发业务规则
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947289"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>如果字段以编程方式更改，则不会发生 OnChange 事件

如果使用 属性以编程方式更改字段，则 *不会发生 OnChange* *事件。*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) 方法。 如果希望 *OnChange* 事件的事件处理程序在设置值后运行，则必须在代码中使用 *formContext.data.entity* 属性 [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) 方法。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
