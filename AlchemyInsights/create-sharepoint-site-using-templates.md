---
title: 在 SharePoint Online SharePoint网站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057956"
---
# <a name="create-sharepoint-sites-using-templates"></a>使用SharePoint创建网站

新式通信或 Teams 网站不支持将网站另存为模板的功能。 有关使用模板的详细信息，请参阅[将 SharePoint 网站保存、下载和上载为模板](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)。

以下是有关在 Sharepoint Online 中将站点或列表保存为模板的一些常见问题/解决方案。 

**"保存网站/列表模板"按钮不可用或缺失**

管理员需要允许自定义脚本才能启用模板功能。 有关详细步骤、示例和注意事项，请参阅 

- [允许或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 不支持“将网站另存为模板”命令，并且在使用 SharePoint Server 发布基础结构的网站上可能会导致问题。

**无法创建网站模板或无法正常运行**

模板可能缺少功能 [，](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) 并且无法激活。 如果无法在当前网站集中激活该功能，则不能使用该网站模板创建网站。

- 检查确认是否有任何列表或库超过了 5000 项的[列表视图限制阈值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)，超出此限制可能会阻止创建网站模板。

- 该网站可能使用了太多资源，因此网站模板超过了 50 MB 的限制。


- 显示使用查找列的列表中的数据时出现问题。 有关详细信息，请参阅[模板生成的列表不显示 SharePoint Online 中正确的查找列表中的数据](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。

有关常见问题和解决方案的更多详细信息，请参阅创建 [和使用网站模板](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。



