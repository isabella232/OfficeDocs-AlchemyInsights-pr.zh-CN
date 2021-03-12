---
title: 自动将电子邮件移动到存档邮箱
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735632"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>自动将电子邮件移动到存档邮箱

下面将设置策略以将用户的旧电子邮件自动移动到存档邮箱：

1. 转到安全 [**&合规性**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **数据管理**  >  **存档**，验证存档邮箱是否已启用用户。 如果尚未启用，请单击警告 **框中的** "启用 **"，然后单击** "是"。
2. 转到 [**Exchange 管理中心，>合规性>保留标记**](https://go.microsoft.com/fwlink/?linkid=2059104)。
3. Choose the + icon then choose **automatically apply to entire mailbox**.
4. 为保留标记分配名称，然后选择"**移动到存档"。** 对于保留期，请输入想要的时间，如 90 天。 单击“**保存**”。
5. 现在创建保留策略：选择 **"保留策略"，** 选择图标以添加新策略。
6. 为保留策略指定名称，然后单击并滚动以查找并添加刚创建的保留标记。 单击“**保存**”。
7. 最后，将保留策略应用于用户的邮箱：仍在 Exchange 管理中心中，转到 **"收件人**  >  **""邮箱"。** Choose all the users who you want to apply the policy to， then choose **Edit** (the pencil icon) .
8. 在对话框中，单击"**邮箱功能"。** 在 **"保留策略**"下，应用刚创建的策略> **保存"**。
9. 有关将策略应用于所有用户的说明，请参阅将 [保留策略应用于邮箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。
