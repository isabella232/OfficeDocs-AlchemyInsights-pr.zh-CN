---
title: 双击 Office 文件无法打开它
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812069"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>双击 Office 文件无法打开它

双击 Office 文件后，您可能会看到该程序打开，但文件本身并不打开。 或者，您可能会收到错误： "将命令发送到程序时出现问题。" 导致此问题的原因有很多，但两个最常见的解决方案是：

- 在 Excel 中，确保未选中 DDE 选项。 可以通过创建新的工作簿，然后选择 " **文件 > 选项" > 高级**"来找到该选项。 在 " **常规** " 部分中，取消选中 " **忽略使用动态数据交换的其他应用程序 (DDE) **"。

- 运行联机修复以还原默认设置。 单击 Windows "开始" 按钮，然后搜索 "控制面板"。 打开 " **控制面板**"，然后转到 " **程序" > "程序和功能**"。 然后右键单击 " **Microsoft Office [Version]** "，然后选择 " **更改 > 联机修复**"。

如果这两种解决方案都不起作用，则可以在支持文章中找到更完整的解决方案列表， [双击 Office 文件将无法打开它](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)。
