---
title: 检查邮箱上的转发地址
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: a67305ed92e181f0ddfc5a929e8fe9631ceefdc99dea34118bc99975461f3868
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005800"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>检查邮箱上的转发地址

有时黑客将用户的电子邮件转发给自己，因此首先我们将检查邮箱上的转发地址和规则。 然后，我们将检查审核日志。 下面将了解如何检查转发地址：

1. 选择 **"用户**  >  **""活动用户"。**
1. 选择帐户遭到入侵的用户。
1. In the flyout that appears， expand **Mail 设置**， and then click **Edit** for **Email forwarding**.
1. 删除你无法识别的任何转发地址。