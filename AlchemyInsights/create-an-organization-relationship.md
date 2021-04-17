---
title: 创建组织关系，以允许你的用户与另一个组织进行协作
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816118"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>创建组织关系，以允许你的用户与另一个组织进行协作

1. 从 Microsoft 365 管理中心主控板中，转到“**管理员**” > “**Exchange**”。
2. 转到“**组织**” > “**共享**”。
3. 在“**组织共享**”下，单击“**新建**”。
4. 在“**新建组织关系**”中的“**关系名称**”框中，为组织关系键入友好名称。
5. 在“**要共享的域**”框中，为允许其查看日历的外部 Office 365 或 Exchange 本地组织键入域。 如果需要输入多个域，请用逗号将域名分隔开。 例如，contoso.com、service.contoso.com。
6. 选中“启用日历忙/闲信息共享”复选框，以开启与列出的域的日历共享。设置日历忙/闲信息的共享级别，并设置可以共享日历忙/闲信息的用户。  

若要设置忙/闲访问级别，请选择以下项目之一：

- **仅包含时间的日历忙/闲信息**
- **包含时间、主题和位置的日历忙/闲信息**  

 若要设置将共享日历忙/闲信息的用户，请选择以下项目之一：

- **组织中的所有人**
- **指定安全组**  

单击“**浏览**”从列表中选取安全组，然后单击“**确定**”。

单击“**保存**”创建组织关系。  

**注意：** 交叉租户配置不支持针对个人联系人的忙/闲查找。 联系人必须包含在全局地址列表中，才能进行忙/闲查找。

**如需全面了解本主题，请阅读：**

- [在 Exchange Online 中创建组织关系](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [在 Exchange Online 中修改组织关系](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [在 Exchange Online 中删除组织关系](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
