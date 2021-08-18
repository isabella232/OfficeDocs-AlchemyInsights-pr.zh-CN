---
title: 自动加密某些Office 365电子邮件
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
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327964"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>自动加密某些Office 365电子邮件

您可以自动加密用户发送给特定外部人员或组织的邮件。 为此，请执行下列步骤：

1. From the [Exchange admin center，](https://outlook.office365.com/ecp/)choose **mail flow > rules**. 
2. 单击"**新建 (+) "** 图标，然后单击"将Office 365 邮件加密 **和权限保护应用于邮件"。**
3. 在 **"** 名称"中，输入规则的名称，例如 *"加密发送到 DrToniRamos@gmail.com"。*
4. 在 **"在应用此规则时"** 中 **，选择"收件人>是此人"。** 
5. 在 **"选择成员**"窗口中，选择要应用加密规则的人的姓名，然后单击"添加 **"。** 
6. 添加完用户后，单击"确定 **"。**
7. 在"执行以下操作 **"字段旁边**，单击"选择 **一个"。** 
8. 在 **RMS 模板下拉菜单中**，选择"加密 **"，** 然后单击"确定 **"。**  (如果未看到此选项，则意味着你的计划不包括自动加密。 但你可以添加它！) 
9. 从此时 (可选选择列表中选择任何可选选项，其中很多选项都可以使用默认设置，以简化) 。
10. 单击“**保存**”。

**重要** 提示：稍后始终可以返回并编辑此规则。

有关创建加密规则的信息，请参阅定义邮件流[规则以加密电子邮件Office 365。](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

