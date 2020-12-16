---
title: 删除 Office 以前的 MSI 版本
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680597"
---
# <a name="remove-prior-msi-versions-of-office"></a>删除 Office 以前的 MSI 版本

在安装 Office 365 专业增强 (，建议先删除 MSI) 版本的 Windows Installer。 下面将说明如何执行此工作：

1. 如果使用 MSI 安装 Office，可以使用 Office 部署工具 (ODT) 卸载 Office。 可以在文件文件中使用 RemoveMSI **configuration.xml** 元素。
1. 按照本文中的说明操作 [：Office 365 安全&合规中心。](https://go.microsoft.com/fwlink/p/?linkid=2077143)