---
title: 导入前修复 .pst 文件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1226
ms.assetid: ''
ms.openlocfilehash: 571f7211915d637f9c193cc453db38b29fc444de
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761893"
---
# <a name="repair-pst-file-before-importing"></a>导入前修复 .pst 文件

在 Outlook 中导入 .pst 文件之前, 请先通过修复文件验证文件是否已损坏:

1. 退出 Outlook。

2. 在 Office 程序`Scanpst.exe`文件夹中查找和运行 (C:\Program Files (x86) \Microsoft Office\root\Office\<version\> or C:\Program Files\Microsoft Office\root\Office\<version\>)。

3. 在**Microsoft Outlook 收件箱修复工具**中, 单击 "**浏览**" 查找 .pst 文件 (例如, 在 C:\Users\\<username\>\AppData\Local\Microsoft\Outlook)。 选择 .pst 文件, 然后单击 "**打开**"。

4. 单击 "**启动**" 开始扫描。

5. 如果在文件中发现错误, 请单击 "**修复**", 然后在修复完成后单击 **"确定"** 。

6. 尝试重新导入 Outlook 中的 .pst 文件。

有关详细信息, 请参阅[修复 outlook 数据文件](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253)和[修复导入 Outlook .pst 文件中的问题](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。
