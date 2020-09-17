---
title: 操作方法-nk2-文件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780049"
---
# <a name="how-to-import-nk2-files"></a>如何导入 nk2 文件 

当您首次启动 Microsoft Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 时，您的昵称缓存 (存储在 *profilename*文件中) 将导入到默认邮件存储区中的隐藏邮件中。

若要将 nk2 文件导入到 Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 中，请确保. nk2 文件位于以下文件夹中：%appdata%\Microsoft\Outlook

**注意**： nk2 文件必须具有与当前 Outlook 2013 或 outlook 2016 配置文件相同的名称。 默认情况下，配置文件名称为 "Outlook"。 若要检查配置文件名称，请按照以下步骤操作： 
1. 单击“开始”****，然后单击“控制面板”****。
2. 双击 " **邮件**"。
3. 在 "邮件设置" 对话框中，选择 " **显示配置文件**"。
4. 选择 "**开始**  >  **运行**"。
5. 在 " **打开** " 框中，键入 *outlook.exe/importnk2*"，然后选择 **" 确定 "**。 

导入 nk2 文件后，该文件的内容将合并到存储在邮箱中的现有昵称缓存中。

**注意**：在下一次启动 outlook 2013、outlook 2016、outlook 2019 或 Outlook for Microsoft 365 时，将使用 .old 文件扩展名将. nk2 文件重命名。 如果要重新导入 nk2 文件，请首先删除 .old 文件扩展名。

有关详细信息，请参阅将 [自动完成列表导入或复制到另一台计算机](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)。