---
title: 面向同一个邮箱的多个活动会话
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769713"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="27ccd-102">面向同一个邮箱的多个活动会话</span><span class="sxs-lookup"><span data-stu-id="27ccd-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="27ccd-103">若要控制 Exchange 资源的使用情况，邮箱有“预算”。</span><span class="sxs-lookup"><span data-stu-id="27ccd-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="27ccd-104">超出预算的异常可以由（但不限于）以下情况触发：</span><span class="sxs-lookup"><span data-stu-id="27ccd-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="27ccd-105">在同一 Outlook Web App 会话中打开几个浏览器选项卡。</span><span class="sxs-lookup"><span data-stu-id="27ccd-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="27ccd-106">面向同一个邮箱的几个活动 Outlook Web App 会话。</span><span class="sxs-lookup"><span data-stu-id="27ccd-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="27ccd-107">一些其他客户端应用程序（Outlook、Outlook Mobile、第三方客户端应用）同时访问邮箱。</span><span class="sxs-lookup"><span data-stu-id="27ccd-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="27ccd-108">长时间运行的操作（如执行搜索请求）将从其他活动邮箱会话执行。</span><span class="sxs-lookup"><span data-stu-id="27ccd-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

