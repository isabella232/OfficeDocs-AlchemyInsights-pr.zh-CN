---
title: 使用 Intune 发送自定义通知
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086154"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>如何向托管 iOS 和 Android 设备的用户发送自定义通知

Intune 的自定义通知由用户公司门户上的应用处理。 然后，应用在该设备上创建推送通知。

以下是支持接收自定义通知的设备先决条件，以及应用随后创建推送通知的设备先决条件：

- 设备必须已安装公司门户应用。  

- 设备必须允许应用公司门户推送通知。 安装或更新应用时，它将提示用户允许通知。

- Android 设备必须已安装 Google Play Services。

- 设备必须注册 Intune。

有关详细信息，包括如何发送消息，请参阅 [功能文档](https://docs.microsoft.com/intune/custom-notifications)。
