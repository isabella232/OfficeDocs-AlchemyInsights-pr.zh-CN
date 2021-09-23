---
title: 升级到 macOS 11.6 Big Sur 后无法添加帐户
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475124"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>升级到 macOS 11.6 Big Sur 后无法添加帐户

升级到 macOS 11.6 后，适用于工作或学校帐户的 OneDrive 或 OneDrive 个人帐户可能不会显示在帐户列表中，并且可能无法从应用登录到另一个帐户。

已针对此问题开发修补程序。 首先，确定运行的是独立版本还是 App Store 版本的 OneDrive：

- 在菜单栏中选择 OneDrive 云 >**帮助和设置** > **偏好设置** > **关于**。 如果版本号不包括 **(单机版)**，则拥有的是该产品的 App Store 版本。

如果使用的是独立版本的 OneDrive，请重启计算机，OneDrive 会自动更新到已解决此问题的内部版本。 若要手动安装生成，请下载此 [.zip 文件](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)，解压缩文件，并将 OneDrive 应用复制到“应用程序”文件夹 (替换现有的 OneDrive 应用)。

如果使用的是 App Store 版本，请考虑安装 OneDrive 的独立版本。 此版本的工作方式与 App Store 版本相同，但允许 Microsoft 更快地向用户提供更新，并将其连接到包含此问题的修补程序的版本。

1. 下载包含修补程序的独立版本 [OneDrive](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)。
2. 解压缩文件，并将 OneDrive 应用复制到“应用程序”文件夹 (替换现有的 OneDrive 应用)。

如果需要使用 App Store 版本，请等待 App Store 发布包含该修补程序的应用版本。 遗憾的是，Microsoft 无法传达从 App Store 发布的固定版本的估计日期。


