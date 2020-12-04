---
title: 如何在 Outlook for Windows 中添加或删除代理
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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571800"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>如何在 Outlook for Windows 中添加或删除代理

若要在 Outlook for Windows 中添加委派，请执行以下操作： 

1. 单击 " **文件** " 选项卡，然后单击 " **帐户设置**"，然后选择 " **委派访问权限**"。
2. 单击 " **添加**"。 如果未显示 " **添加** "，则 Outlook 和 Exchange 之间可能不存在活动连接。 Outlook 状态栏显示连接状态。
3. 键入要指定为代理的人员的姓名，或在搜索结果列表中搜索并选择名称。

    > [!NOTE]
    > 代理必须是组织的 Exchange 全局地址列表中 (GAL) 的人员。
4. 单击 " **添加** "，然后单击 **"确定"**。
5. 在 " **代理权限** " 对话框中，接受默认权限设置或选择 "Exchange 文件夹的自定义访问级别"。

    - 如果代理需要仅处理会议请求和响应的权限，则默认权限设置（如代理）将 **接收发送给我的与会议相关的邮件的副本** ，这是足够的。 您可以将 **收件箱** 权限设置保留为 **无**。 会议请求和响应将直接转到代理的 "收件箱"。

    > [!NOTE]
    > 默认情况下，授予代理 **(可以读取、创建和修改** 对 " **日历** " 文件夹的项目) 权限。 当代理代表您响应会议时，它会自动添加到 " **日历** " 文件夹中。

5. 若要发送邮件以通知代理已更改的权限，请选中 " **自动向代理发送邮件概述这些权限** " 复选框。
6. 如果需要，请选中 " **代理可以查看我的私人性质项目** " 复选框。

    > [!IMPORTANT]
    > 此设置会影响所有 Exchange 文件夹。 这包括所有邮件、联系人、日历、任务、便笺和日记文件夹。 无法在仅指定的文件夹中授予对私人性质项目的访问权限。

7. 选择“**确定**”。

    > [!NOTE]
    >
    > - 使用 "代表发送" 权限发送的邮件在 " **发件人**" 旁边包含代理和您的姓名。 使用 "代理发送" 权限发送邮件时，将只显示您的名称。
    > - 一旦将某人添加为代理人，他们就可以将您的 Exchange 邮箱添加到其 Outlook 配置文件中。 有关说明，请参阅 [管理其他人的邮件和日历项目](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)。

若要在 Outlook for Windows 中删除代理，请执行以下操作：

1. 单击 " **文件** " 选项卡。
2. 单击 " **帐户设置** "，然后单击 " **代理访问**"。
3. 选择要更改其权限的代理人的名称，然后单击 " **删除** " 后再单击 **"确定"**。
