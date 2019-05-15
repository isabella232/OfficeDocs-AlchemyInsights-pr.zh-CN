---
title: 访问服务退休
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973900"
---
# <a name="access-services-retirement"></a>访问服务退休

正如我们最初在 MC97576 中宣布的那样, 在2017年3月, 并持续与过去一年的通信。将从 Office 365 中停用 Access 服务。 此过程的下一阶段将是删除使用 SharePoint 列表作为其基础数据存储的 Access Web 数据库。

## <a name="how-does-this-affect-me"></a>这对我有何影响？

从2019年6月起, 我们将停止在 SharePoint Online 中创建新的 Access 数据库, 并在4月2020关闭服务和任何剩余的应用。

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>为此更改做准备需要做些什么？

我们鼓励你为组织的 Access web 数据库创建过渡计划。 管理员可以使用[SharePoint access 应用程序扫描](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0)程序获取网站正在使用的 Access 应用程序的清单。 

有几种方法可以迁移 Access web 数据库数据:

- 导入到本地 Access 数据库 (。.ACCDB) 或 Excel 文件。
- 我们还建议研究 Microsoft PowerApps 作为替代平台, 以便为 web 和移动设备创建无代码业务解决方案。