---
title: 配置发送给用户的隔离通知
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
- "9002531"
- "7375"
ms.openlocfilehash: 3e3e350f74b19420155c29cb282f065e7db6d4d7
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735528"
---
# <a name="configure-quarantine-notifications-sent-to-users"></a><span data-ttu-id="fe422-102">配置发送给用户的隔离通知</span><span class="sxs-lookup"><span data-stu-id="fe422-102">Configure quarantine notifications sent to users</span></span>

<span data-ttu-id="fe422-103">若要向用户发送有关隔离内容的通知：</span><span class="sxs-lookup"><span data-stu-id="fe422-103">To send notifications to your users about what's in quarantine:</span></span>

1. <span data-ttu-id="fe422-104">In the admin center， navigate to **admin centers**  >  **Exchange**  >  **Protection**  >  **spam filter**.</span><span class="sxs-lookup"><span data-stu-id="fe422-104">In the admin center, navigate to **admin centers** > **Exchange** > **Protection** > **spam filter**.</span></span>
2. <span data-ttu-id="fe422-105">选择要打开通知的垃圾邮件筛选策略。</span><span class="sxs-lookup"><span data-stu-id="fe422-105">Select the spam filter policy for which you want to turn on notifications.</span></span>
3. <span data-ttu-id="fe422-106">在右侧窗格中，选择" **配置最终用户垃圾邮件通知"** 链接。</span><span class="sxs-lookup"><span data-stu-id="fe422-106">In the right pane, choose the **Configure End-user spam notifications** link.</span></span>
4. <span data-ttu-id="fe422-107">In the next dialog box， choose **Enable end-user spam notifications**.</span><span class="sxs-lookup"><span data-stu-id="fe422-107">In the next dialog box, choose **Enable end-user spam notifications**.</span></span> <span data-ttu-id="fe422-108">选择为此策略启用垃圾邮件通知。</span><span class="sxs-lookup"><span data-stu-id="fe422-108">Choose to enable spam notifications for this policy.</span></span>
5. <span data-ttu-id="fe422-109">在 **"每两天发送最终用户垃圾邮件 () ，** 指定发送用户垃圾邮件通知的发送时间。</span><span class="sxs-lookup"><span data-stu-id="fe422-109">In **Send end-user spam notifications every (days)**, specify how often to send user spam notifications.</span></span> <span data-ttu-id="fe422-110">默认值为 3 天。</span><span class="sxs-lookup"><span data-stu-id="fe422-110">The default is 3 days.</span></span> <span data-ttu-id="fe422-111">您可以指定一个介于 1 到 15 天之间的值。</span><span class="sxs-lookup"><span data-stu-id="fe422-111">You can specify between 1 and 15 days.</span></span> <span data-ttu-id="fe422-112">例如，如果您指定 7 天，则该通知将包括在过去 7 天内预期发送给该用户但实际发送到垃圾邮件隔离邮箱的所有邮件列表。</span><span class="sxs-lookup"><span data-stu-id="fe422-112">If you specify 7 days, for example, the notification will include a list of all messages intended for that user within the past 7 days that were sent to the spam quarantine instead.</span></span>
6. <span data-ttu-id="fe422-113">在 **"通知** 语言"中，选择为此策略编写用户垃圾邮件通知的语言。</span><span class="sxs-lookup"><span data-stu-id="fe422-113">In **Notification language** choose the language in which to write user spam notifications for this policy.</span></span>
7. <span data-ttu-id="fe422-114">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="fe422-114">Choose **Save**.</span></span>
