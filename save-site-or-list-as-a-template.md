---
title: 将网站或列表另存为模板
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31043995"
---
# <a name="save-site-or-list-as-a-template"></a>将网站或列表另存为模板

SharePoint 网站模板是围绕特定的业务需要设计的预制定义。 有关详细信息, 请参阅[使用模板创建不同种类的 SharePoint 网站](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。

下面是有关在 SharePoint Online 中将网站或列表保存为模板的一些常见问题/解决方案。

"**保存网站/列表模板" 按钮不可用或缺失**。 

- 管理员将需要允许自定义脚本启用模板功能。 有关详细步骤、示例和注意事项, 请参阅[Allow or 预防自定义脚本](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)。


- "将网站另存为模板" 命令不受支持, 并且可能会在使用 SharePoint Server 发布基础结构的网站上出现问题。


**网站模板无法创建或无法正常工作**

- 模板可能缺少[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx), 无法激活。 如果在当前网站集中无法激活该功能, 则不能使用网站模板创建网站。


- 检查以查看是否有任何列表或库超出了5000个项目的[列表视图限制阈值](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), 因为这可能会阻止创建网站模板。


- 网站可能使用过多的资源, 因此网站模板超过了 50 mb 的限制。


- 显示使用查阅列的列表中的数据时出现问题。 有关详细信息, 请参阅[模板生成的列表不会在 SharePoint Online 中显示正确的查找列表中的数据](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。


有关常见问题和解决方案的更多详细信息, 请参阅[创建和使用网站模板](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。

