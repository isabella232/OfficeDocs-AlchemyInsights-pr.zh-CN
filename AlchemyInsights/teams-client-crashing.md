---
title: Teams 客户端发生了故障？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030515"
---
# <a name="teams-client-crashing"></a>Teams 客户端发生了故障？

如果 Teams 客户端发生了故障，请尝试执行以下操作：

- 如果使用的是 Teams 桌面应用，请[确保应用已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- 确保所有 [Office 365 URL 和地址范围](https://docs.microsoft.com/microsoftteams/connectivity-issues)都可访问。

- 使用管理员帐户登录，然后检查[服务运行状况仪表板](https://docs.microsoft.com/office365/enterprise/view-service-health)，以确认是否没有任何故障或服务降级。

 - 最后，可以尝试清除 Teams 客户端缓存：

    1.  完全退出 Microsoft Teams 桌面客户端。 可以右键单击图标托盘中的“Teams”****，然后单击“退出”****，也可以运行“任务管理器”，并完全终止进程。

    2.  转到“文件资源管理器”，然后键入“%appdata%\Microsoft\teams”。

    3.  进入目录后，便会看到以下几个文件夹：

         - 在“应用程序缓存”**** 中，转到“缓存”，然后删除“缓存”位置 (%appdata%\Microsoft\teams\application cache\cache) 中的任何文件。

        - 在“Blob_storage”****(%appdata%\Microsoft\teams\blob_storage) 中，删除所有文件。

        - 在“缓存”****(%appdata%\Microsoft\teams\Cache) 中，删除所有文件。

        - 在“数据库”****(%appdata%\Microsoft\teams\databases) 中，删除所有文件。

        - 在“GPUCache”****(%appdata%\Microsoft\teams\GPUcache) 中，删除所有文件。

        - 在“IndexedDB”****(%appdata%\Microsoft\teams\IndexedDB) 中，删除 .db 文件。

        - 在“本地存储”****(%appdata%\Microsoft\teams\Local Storage) 中，删除所有文件。

        - 最后，在“tmp”****(%appdata%\Microsoft\teams\tmp) 中，删除所有文件。

    4. 重启 Teams 客户端。