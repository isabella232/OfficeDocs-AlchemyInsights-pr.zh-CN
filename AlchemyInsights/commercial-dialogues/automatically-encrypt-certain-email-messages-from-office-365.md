---
title: 自动加密来自 Office 365 的某些电子邮件
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
ms.openlocfilehash: e050074f26025906561237c9ef487ed4743f93b1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322239"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>自动加密来自 Office 365 的某些电子邮件

1. From the [Exchange admin center，](https://outlook.office365.com/ecp/)choose **mail flow > rules**. 
2. 单击"**新建 (+) "** 图标，然后单击"将Office 365 邮件加密 **和权限保护应用于邮件"。**
3. 在 **"** 名称"中，输入规则的名称，如"*加密所有邮件"。*
4. 在 **"在应用此规则时"中**，选择 **"[应用于所有邮件]"。** 
5. 在"执行以下操作 **"字段旁边**，单击"选择 **一个"。** 
6. 在 **RMS 模板下拉菜单中**，选择"加密 **"，** 然后单击"确定 **"。**  (如果未看到此选项，则意味着你的计划不包括自动加密。 但你可以添加它！) 
7. 选中" **使用严重性级别审核此规则** "复选框，然后选择所需的级别。 如果你的公司有合同义务发送所有加密的电子邮件，建议将级别设置为 **"高"。**
8. 在 **"为此规则选择模型"下，单击**"**强制"。** 
9. 从此时 (可选选择列表中选择任何可选选项，其中很多选项都可以使用默认设置，以简化) 。
10. 单击“**保存**”。

**重要** 提示：稍后始终可以返回并编辑此规则。

有关创建加密规则的信息，请参阅定义邮件流[规则以加密电子邮件Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

