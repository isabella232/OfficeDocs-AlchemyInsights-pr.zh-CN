---
title: 为混合环境配置邮件加密
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 59360a040fe413e92cd880b1225b9006384a823f6e8abeb7ef922949b9a874fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035212"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>为混合环境配置邮件加密

对于混合Exchange环境，本地用户可以使用 Office 邮件加密 (OME) 仅在电子邮件通过 Exchange Online 路由时发送加密Exchange Online。

若要使用 OME 加密电子邮件，请执行以下步骤：

1. 使用 ["混合配置"](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) 向导设置混合环境。 设置加密不需要任何特殊步骤。
2. [像通常一样设置邮件流](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) 规则进行加密。


