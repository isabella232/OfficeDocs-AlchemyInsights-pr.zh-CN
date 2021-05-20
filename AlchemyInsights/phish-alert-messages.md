---
title: 2491 警报来自"由于租户或用户覆盖而传递的网络钓鱼"策略的电子邮件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544568"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="07b5d-102">警报来自"由于租户或用户覆盖而传递的网络钓鱼"策略的电子邮件</span><span class="sxs-lookup"><span data-stu-id="07b5d-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="07b5d-103">名为"由于租户或用户覆盖而送达的网络钓鱼"的默认警报策略已推出给使用 Microsoft Defender 的租户，Office 365 P1 和 P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="07b5d-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="07b5d-104">如果您收到此警报，以下是要调查的步骤：</span><span class="sxs-lookup"><span data-stu-id="07b5d-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="07b5d-105">从警报消息中，单击 **"查看警报**"以转到安全与合规中心&警报"页面。</span><span class="sxs-lookup"><span data-stu-id="07b5d-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="07b5d-106">选择警报以查看查看邮件列表或在资源管理器 **中查看邮件的选项**。 </span><span class="sxs-lookup"><span data-stu-id="07b5d-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="07b5d-107">这两个选项都使你可以查看邮件的详细信息，其中包括邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="07b5d-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="07b5d-108">请注意，威胁资源管理器链接将自动筛选与警报条件匹配的邮件。</span><span class="sxs-lookup"><span data-stu-id="07b5d-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="07b5d-109">你可能需要在威胁资源管理器中调整日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="07b5d-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="07b5d-110">由于手动配置的覆盖，传送了网络钓鱼邮件：</span><span class="sxs-lookup"><span data-stu-id="07b5d-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="07b5d-111">用户设置的允许发件人或域。</span><span class="sxs-lookup"><span data-stu-id="07b5d-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="07b5d-112">管理员在反垃圾邮件策略中设置的允许发件人或域。</span><span class="sxs-lookup"><span data-stu-id="07b5d-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="07b5d-113">连接筛选器策略中允许的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="07b5d-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="07b5d-114">邮件流规则 (也称为传输规则) 配置为允许邮件使用的邮件流规则。</span><span class="sxs-lookup"><span data-stu-id="07b5d-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="07b5d-115">如果您认为邮件被错误地标记为网络钓鱼邮件，请使用 Outlook[报告邮件外接程序](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)将邮件示例提交给 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="07b5d-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
