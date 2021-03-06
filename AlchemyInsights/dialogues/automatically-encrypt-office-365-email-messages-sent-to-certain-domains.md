---
title: 自动加密发送到特定域的 Office 365 电子邮件
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509677"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>自动加密发送到特定域的 Office 365 电子邮件

1. 从 [Exchange 管理中心](https://outlook.office365.com/ecp/)， **选择邮件流>规则**。 
2. 单击 **"新建 (+)** 图标，然后单击"将 Office **365** 邮件加密和权限保护应用于邮件"。
3. 在 **"名称**"中，输入规则的名称，例如加密发送到 *contoso.com。*
4. 在 **"如果应用此规则"中**，选择"域 **>收件人。** 
5. 输入域的名称，例如 **contoso.com。**
6. 单击 **" (+)** 图标，然后单击"**确定"。**
7. 在"**执行以下操作"字段旁边**，单击"**选择一个"。** 
8. 在 **RMS 模板** 下拉菜单中，**选择"加密**"，然后单击"**确定"。**  (如果看不到此选项，这意味着你的计划不包括自动加密。 但你可以添加它！) 
9. 从 (可选选择列表中选择任何可选选项，许多可选选择都可以通过默认设置进行选择，以简化) 。
10. 单击“**保存**”。

> [!IMPORTANT]
> 稍后始终可以返回并编辑此规则。

有关创建加密规则的信息，请参阅["定义邮件流规则以加密 Office 365 中的电子邮件](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)"