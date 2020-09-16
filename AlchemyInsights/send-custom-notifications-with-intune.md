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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720636"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>如何向托管的 iOS 和 Android 设备的用户发送自定义通知

适用于 Intune 的自定义通知由用户设备上的公司门户应用程序处理。 然后，应用在该设备上创建推送通知。

以下是支持接收自定义通知的设备先决条件，并且应用程序将创建推送通知：

- 设备必须已安装公司门户应用程序。  

- 设备必须允许公司门户应用发送推送通知。 在安装或更新应用程序时，它将提示用户允许通知。

- Android 设备必须安装 Google Play Services。

- 必须使用 Intune 注册设备。

有关详细信息，包括如何发送邮件，请参阅 [功能文档](https://docs.microsoft.com/intune/custom-notifications)。
