---
title: 修复连接策略
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
- "9000760"
- "7391"
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314834"
---
# <a name="fix-connection-policy"></a>修复连接策略

电子邮件被标记为安全并传递到用户的收件箱，因为源 IP 地址在默认连接筛选器策略中标记为安全。 若要查看策略，请执行以下步骤：

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> ， go to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **Anti-spam** in the **Policies** section.

   若要直接转到“**反垃圾邮件策略**”页面，请使用 <https://security.microsoft.com/antispam>。

2. 在 **"反垃圾邮件策略**"页上，单击该策略的名称 ("默认) 选择名为"连接筛选器策略"的策略。

3. 在出现的详细信息飞出控件中，单击"连接筛选"部分 **中的** "编辑 **连接筛选器策略** "。

4. 查看"始终允许来自以下 **IP** 地址或地址范围的邮件"部分中的条目，并查看是否 **选择了"打开安全** 列表"。

   **注意**：Microsoft 订阅受信任发件人的第三方源。 如果启用安全列表，这些受信任的发件人不会错误地标记为垃圾邮件。 建议选择此选项，因为这样可以减少被归类为垃圾邮件 (垃圾邮件的误报) 数量。

有关详细信息，请参阅[配置连接筛选](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)。
