---
title: 2491通知电子邮件来自 "由于租户或用户替代而发送的网络钓鱼" 策略
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758898"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="ea57d-102">通知来自 "由于租户或用户替代的网络钓鱼传递" 策略的电子邮件</span><span class="sxs-lookup"><span data-stu-id="ea57d-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="ea57d-103">一个名为 "由于租户或用户替代而发送的网络钓鱼" 的默认通知策略已通过 Office 365 ATP P1 和 P2 许可证推出给租户。</span><span class="sxs-lookup"><span data-stu-id="ea57d-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="ea57d-104">如果你收到此通知，请查看以下步骤：</span><span class="sxs-lookup"><span data-stu-id="ea57d-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="ea57d-105">在警告消息中，单击 "**查看通知**" 以转到安全 & 合规性中心中的 "**通知**" 页面。</span><span class="sxs-lookup"><span data-stu-id="ea57d-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="ea57d-106">选择警报以查看**查看邮件列表**的选项或**查看资源管理器中的邮件**。</span><span class="sxs-lookup"><span data-stu-id="ea57d-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="ea57d-107">这两个选项都将您带到邮件的详细信息，其中包括邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="ea57d-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="ea57d-108">请注意，威胁资源管理器链接将自动筛选符合警报条件的邮件。</span><span class="sxs-lookup"><span data-stu-id="ea57d-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="ea57d-109">您可能需要在威胁资源管理器中调整日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="ea57d-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="ea57d-110">由于手动配置的替代，已传递网络钓鱼邮件：</span><span class="sxs-lookup"><span data-stu-id="ea57d-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="ea57d-111">用户设置的允许发件人或域。</span><span class="sxs-lookup"><span data-stu-id="ea57d-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="ea57d-112">由管理员在反垃圾邮件策略中设置的允许发件人或域。</span><span class="sxs-lookup"><span data-stu-id="ea57d-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="ea57d-113">连接筛选器策略中允许的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ea57d-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="ea57d-114">配置为允许中的邮件的邮件流规则（也称为传输规则）。</span><span class="sxs-lookup"><span data-stu-id="ea57d-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="ea57d-115">如果您认为邮件被错误地标记为网络钓鱼，请使用 Outlook[报告邮件外接程序](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)将邮件示例提交给 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="ea57d-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
