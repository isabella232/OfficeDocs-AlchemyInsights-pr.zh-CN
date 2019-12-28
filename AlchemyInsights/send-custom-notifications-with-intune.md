---
title: 使用 Intune 发送自定义通知
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886847"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="b5ab5-102">如何向托管的 iOS 和 Android 设备的用户发送自定义通知</span><span class="sxs-lookup"><span data-stu-id="b5ab5-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="b5ab5-103">适用于 Intune 的自定义通知由用户设备上的公司门户应用程序处理。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="b5ab5-104">然后，应用在该设备上创建推送通知。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="b5ab5-105">以下是支持接收自定义通知的设备先决条件，并且应用程序将创建推送通知：</span><span class="sxs-lookup"><span data-stu-id="b5ab5-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="b5ab5-106">设备必须已安装公司门户应用程序。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="b5ab5-107">设备必须允许公司门户应用发送推送通知。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="b5ab5-108">在安装或更新应用程序时，它将提示用户允许通知。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="b5ab5-109">Android 设备必须安装 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="b5ab5-110">必须使用 Intune 注册设备。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="b5ab5-111">有关详细信息，包括如何发送邮件，请参阅[功能文档](https://docs.microsoft.com/intune/custom-notifications)。</span><span class="sxs-lookup"><span data-stu-id="b5ab5-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
