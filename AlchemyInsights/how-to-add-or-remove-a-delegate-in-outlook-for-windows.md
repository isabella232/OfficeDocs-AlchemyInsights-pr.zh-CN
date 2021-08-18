---
title: 如何为用户添加或删除Outlook代理Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329015"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>如何为用户添加或删除Outlook代理Windows

若要在 Outlook 中添加Windows： 

1. 单击"文件 **"** 选项卡 **，后跟**"帐户设置"，然后选择"委派 **访问"。**
2. 单击"添加 **"。** 如果未显示 **Add，** 则活动连接可能不存在于 Outlook 和 Exchange。 "Outlook"状态栏显示连接状态。
3. 键入要指定为代理的人的名称，或搜索并选择搜索结果列表中的姓名。

    **注意**：代理必须是组织全局地址列表Exchange GAL (人员) 。
4. 单击"**添加"，** 然后单击"**确定"。**
5. 在"**委派权限"** 对话框中，接受默认权限设置，或选择文件夹的自定义Exchange级别。

    - 如果代理仅需要处理会议请求和响应的权限，则默认权限设置（如 **Delegate）** 接收发送给我的会议相关邮件的副本就足够了。 可以将收件箱权限 **设置保留** 为"无 **"。** 会议请求和响应将直接转到代理人的收件箱。

    **注意**：默认情况下，代理被授予编辑器 (**读取** 、创建和修改项目) 日历 **文件夹的权限** 。 当代理代表你响应会议时，它会自动添加到你的 **日历** 文件夹中。

5. 若要发送邮件以通知代理已更改的权限，请选中"自动发送邮件给委派总结 **这些权限** "复选框。
6. 如果需要，请选中" **代理可以看到我的私人项目"** 复选框。

    **重要** 提示：此设置影响所有Exchange文件夹。 这包括所有邮件、联系人、日历、任务、便笺和日记文件夹。 无法仅向指定文件夹中的私有项目授予访问权限。

7. 选择"确定"。

    **注意**：
    - 使用"代表发送"权限发送的邮件包括代理和"From"旁边的 **姓名**。 当使用"发送方式"权限发送邮件时，只显示您的姓名。
    - 将某人添加为代理后，他们可以将你的Exchange添加到其Outlook配置文件。 有关说明，请参阅 [管理其他人的邮件和日历项目](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)。

若要删除 Outlook 中的Windows：

1. 单击"文件 **"** 选项卡。
2. 单击"**帐户设置** 后跟"**委派访问"。**
3. 选择要更改其权限的代理的名称，然后单击"删除"，然后单击"确定 **"。** 
