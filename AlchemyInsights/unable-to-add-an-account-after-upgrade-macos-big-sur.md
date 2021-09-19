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
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446720"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>升级到 macOS 11.6 Big Sur 后无法添加帐户

升级到 macOS 11.6 后，适用于工作或学校帐户的 OneDrive 或 OneDrive 个人帐户可能不会显示在帐户列表中，并且可能无法从应用登录到另一个帐户。

这是与 macOS 11.6 升级相关的新问题。 在问题解决之前，你可以从 Web 或移动设备访问 OneDrive 内容。 Microsoft 正在与 Apple 合作来还原 OneDrive 功能。

还可以使用终端手动启动缺少的 OneDrive 实例。 

**注意**：此解决方法仅在 OneDrive 重启（通过计算机重新启动或 OneDrive 应用更新）之前有效。

如果缺少的实例是个人帐户，请打开终端并输入：

`open "/Applications/OneDrive.app" --new --args /client=Personal`

如果缺少的实例是工作或学校帐户，请打开终端并输入：

`open "/Applications/OneDrive.app" --new --args /client=Business1`

