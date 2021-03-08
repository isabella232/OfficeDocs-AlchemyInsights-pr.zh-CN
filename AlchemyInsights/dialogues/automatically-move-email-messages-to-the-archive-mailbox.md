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
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522356"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>自动将电子邮件移动到存档邮箱

下面是如何设置策略以将用户的旧电子邮件自动移动到存档邮箱：

1. 转到 [**"安全&**](https://go.microsoft.com/fwlink/p/?linkid=2077143)合规性数据管理存档"，验证存档邮箱  >    >  是否已启用用户。 如果尚未启用， **请在警告框中** 单击" **启用"，** 然后单击"是"。
2. 转到 [**Exchange 管理中心>合规性管理>保留标记**](https://go.microsoft.com/fwlink/?linkid=2059104)。
3. 选择 + 图标，然后选择 **自动应用于整个邮箱**。
4. 为保留标记分配名称，然后选择"**移动到存档"。** 对于保留期，输入您想要的时间，如 90 天。 单击“**保存**”。
5. 现在创建保留策略：选择 **保留策略**，选择图标以添加新策略。
6. 为保留策略分配名称，然后单击并滚动以查找并添加刚创建的保留标记。 单击“**保存**”。
7. 最后，将保留策略应用于用户的邮箱：仍在 Exchange 管理中心中，转到 **收件人**  >  **邮箱**。 选择要应用策略的所有用户，然后选择"编辑 (铅笔图标) 。 
8. 在对话框中，单击 **邮箱功能**。 在 **"保留策略**"下，应用刚创建的策略> **保存**。
9. 有关将策略应用于所有用户的说明，请参阅"将保留策略应用于[邮箱"。](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
