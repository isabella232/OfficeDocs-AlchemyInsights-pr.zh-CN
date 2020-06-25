---
title: 创建共享策略，以允许你的用户与组织外部的人员共享其日历
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44853992"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>创建共享策略，以允许你的用户与组织外部的人员共享其日历

1. 从 Microsoft 365 管理中心主控板中，转到“**管理员**” > “**Exchange**”。
2. 转到“**组织**” > “**共享**”。
3. 在列表视图中的“**单个共享**”下，单击“**新建**”。
4. 在“**新建共享策略**”中，在“**策略名称**”框中为共享策略键入一个友好名称。
5. 单击“**添加**”定义策略的共享规则。
6. 在“共享规则”中，选择以下选项之一以指定要共享的域：
    - **与所有域共享**
    - **与特定域共享**
8. If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.
9. 若要指定可共享的信息，请选中“共享日历文件夹”复选框，然后选择以下选项之一：
    - **仅包含时间的日历忙/闲信息**
    - **包含时间、主题和位置的日历忙/闲信息**
    - **所有日历约会信息，包括时间、主题、位置和标题**
11. 单击“保存”设置共享策略的规则。
12. 如果希望将该共享策略设置为你组织中所有用户的新默认共享策略，可选中“**将该策略作为我的默认共享策略**”复选框。
13. 单击“**保存**”创建共享策略。  

**如需全面了解本主题，请阅读：**

- [在 Exchange Online 中创建共享策略](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [将共享策略应用于 Exchange Online 中的邮箱](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [修改、禁用或删除 Exchange Online 中的共享策略](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)