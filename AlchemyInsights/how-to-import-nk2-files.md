---
title: how-to-import-nk2-files
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
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043196"
---
# <a name="how-to-import-nk2-files"></a>如何导入 .nk2 文件 

首次启动 Microsoft Outlook 2013、Outlook 2016、Outlook 2019 或 Microsoft 365 专属 Outlook 时，存储在 *profilename*.nk2 文件) 中的昵称缓存 (将导入到默认邮件存储中的隐藏邮件中。

若要将 .nk2 文件导入 Outlook 2013、Outlook 2016、Outlook 2019 或 Microsoft 365 专属 Outlook，请确保 .nk2 文件位于以下文件夹中：%appdata%\Microsoft\Outlook

**注意**：.nk2 文件的名称必须与当前 Outlook 2013 或 Outlook 2016相同。 默认情况下，配置文件名称为"Outlook"。 若要检查配置文件名称，请按照以下步骤操作： 
1. 单击“开始”，然后单击“控制面板”。
2. 双击"邮件 **"。**
3. 在"邮件设置"对话框中，选择"**显示配置文件"。**
4. 选择“开始” > “运行”。
5. 在"**打开"** 框中 *，outlook.exe /importnk2"，* 然后选择"确定 **"。** 

导入 .nk2 文件后，该文件的内容将合并到邮箱中存储的现有昵称缓存中。

**注意**：下次启动 Outlook 2013、Outlook 2016、Outlook 2019 或 Microsoft 365 专属 Outlook 时，.nk2 文件将重命名为 .old 文件扩展名。 如果要重新导入 .nk2 文件，请首先删除 .old 文件扩展名。

有关详细信息，请参阅 [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)。