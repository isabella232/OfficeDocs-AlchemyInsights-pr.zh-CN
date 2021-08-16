---
title: 用于视频播放的 CDN
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071106"
---
# <a name="cdn-used-for-video-playback"></a>用于视频播放的 CDN

来自 Stream 和外部应用的实时事件或来自 Yammer/Teams 的设备实时事件将自动使用 Azure CDN。 上传到 Stream 的点播视频尚未使用 Azure CDN 进行播放。 将从与租户所在地理区域中的租户关联的 Azure 媒体服务原始服务器播放 Stream 中的非实时视频。 有关详细信息，请参阅：

- [用于视频播放的 CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
