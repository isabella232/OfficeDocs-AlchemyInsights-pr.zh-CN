---
title: 解决 Mac 上的 MDATP 安装问题
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735669"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>解决 Mac 上的 MDATP 安装问题

如果手动安装失败，则 **安装向导的** "摘要"页将显示以下错误：

"在安装过程中出错。 安装程序遇到导致安装失败的错误。 请与软件制造商联系寻求帮助。"

对于 MDM 部署，页面也显示常规安装失败。

尽管我们不会向最终用户显示确切的错误，但我们在 **/Library/Logs/Microsoft/mdatp/install.log** 中日志文件安装进度进行跟踪。 每个安装会话都附加到此日志文件。 若要仅输出上次安装会话，请使用 `sed` 。

若要了解更多信息，请参阅 [解决 Microsoft Defender ATP for Mac 的安装问题](https://go.microsoft.com/fwlink/?linkid=2144615)。
