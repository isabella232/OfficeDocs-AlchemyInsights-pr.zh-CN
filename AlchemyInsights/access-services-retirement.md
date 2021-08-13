---
title: Access Services 停用
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938685"
---
# <a name="access-services-retirement"></a>Access Services 停用

正如我们最初在 MC97576 中于 2017 年 3 月宣布的，并在过去一年继续Access Services即将停用。 此过程的下一个阶段是删除使用列表作为基础数据存储SharePoint Access Web 数据库。

**这对我有何影响？**

从 2019 年 6 月开始，我们将停止在 SharePoint Online 中新建 Access 数据库，并将于 2020 年 4 月关闭该服务和任何其他应用。

**为准备此更改，我需要做什么？**

我们鼓励您为组织的 Access Web 数据库创建转换计划。 管理员可以使用 SharePoint [Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)应用程序扫描程序获取网站使用的 Access 应用的清单。

有几种方法可以迁移 Access Web 数据库数据：

- 导入到本地 Access 数据库 (。ACCDB) 或Excel文件。
- 我们还建议Microsoft PowerApps作为备用平台来为 Web 和移动设备创建无代码业务解决方案。