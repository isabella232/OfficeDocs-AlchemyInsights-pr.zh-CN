---
title: 将 Microsoft Edge 设置为 macOS 设备上的默认浏览器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426771"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>将 Microsoft Edge 设置为 macOS 设备上的默认浏览器

使用以下两种方法之一将 Microsoft Edge 设置为默认浏览器：

方法 1：使用已将 Microsoft Edge 设置为默认浏览器的 macOS 映像刷新设备。

方法 2：将 DefaultBrowserSettingEnabled 策略设置为提示用户将 Microsoft Edge 设置为默认浏览器。

这两种方法都允许用户更改默认浏览器。 因此，我们建议你即使使用了方法 1，也部署 DefaultBrowserSettingEnabled 策略。 如果用户在部署策略后更改了默认浏览器，则该策略会提示用户将默认浏览器设置回 Microsoft Edge。
