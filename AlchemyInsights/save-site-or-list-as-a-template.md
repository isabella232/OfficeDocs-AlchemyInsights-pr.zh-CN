---
title: 将网站或列表另存为模板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109194"
---
# <a name="save-site-or-list-as-a-template"></a>将网站或列表另存为模板

SharePoint 网站模板是围绕特定的业务需要设计的预制定义。 有关详细信息，请参阅使用[模板创建不同类型的SharePoint网站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。

以下是有关在 SharePoint Online 中将站点或列表保存为模板的一些常见问题/解决方案。

**"保存网站/列表模板"按钮不可用或缺失**。 

- 管理员需要允许自定义脚本才能启用模板功能。 有关详细步骤、示例和注意事项，请参阅 [允许或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


- 不支持“将网站另存为模板”命令，并且在使用 SharePoint Server 发布基础结构的网站上可能会导致问题。


**无法创建网站模板或无法正常运行**

- 模板可能缺少功能 [，](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) 并且无法激活。 如果无法在当前网站集中激活该功能，则不能使用该网站模板创建网站。


- 检查确认是否有任何列表或库超过了 5000 项的[列表视图限制阈值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)，超出此限制可能会阻止创建网站模板。


- 网站可能使用了过多的资源，因此网站模板超出了 50 MB (MB) 限制。


- 显示使用查找列的列表中的数据时出现问题。 有关详细信息，请参阅[模板生成的列表不显示来自 SharePoint Online 中正确查找列表的数据](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。


有关常见问题和解决方案的更多详细信息，请参阅创建 [和使用网站模板](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。

