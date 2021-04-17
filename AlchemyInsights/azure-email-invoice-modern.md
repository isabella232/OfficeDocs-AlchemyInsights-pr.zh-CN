---
title: 新式 Azure 电子邮件发票
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820816"
---
# <a name="email-invoicing-in-azure"></a>Azure 中的电子邮件发票

必须在帐单配置文件或其帐单帐户中拥有所有者或参与者角色，才能更新其电子邮件发票首选项。 选择加入后，在帐单配置文件中拥有所有者、参与者、读者和发票管理员角色的所有用户都将在电子邮件中获取发票。

1. 登录到 [Azure 门户](https://portal.azure.com/)。
2. 搜索“**成本管理 + 帐单**”。
3. 从左侧选择“**发票**”，然后从页面顶部选择“**使用电子邮件发送发票**”。
4. 如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“**选择加入**”。

5. 选择 **“更新”**。
6. 如果你有多个帐单配置文件，请选择帐单配置文件，然后选择“**选择加入**”。

对于 MCA 或 MPA 帐单配置文件，你可通过向其分配发票管理员角色，授予其查看、下载和支付发票的权限。 如果你选择要在电子邮件中获取发票，用户也会在电子邮件中获取发票。

1. 登录到 [Azure 门户](https://portal.azure.com/)。
2. 搜索“**成本管理 + 帐单**”。
3. 从左侧选择“**计费对象信息**”。 从“帐单配置文件”列表中，选择要为其分配发票管理员角色的帐单配置文件。
4. 从左侧选择 “**访问控制（IAM）**” ，然后选择从页面顶部选择“**添加**”。

在“角色”下拉列表中，选择“**发票管理员**”。 输入要向其授予访问权限的用户的电子邮件地址。 选择“**保存**”以分配角色。
