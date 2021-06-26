---
title: 通过 Microsoft 365 中继电子邮件
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117973"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a5545-102">设置多功能设备或应用程序以发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="a5545-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a5545-103">若要了解有关选项和步骤的详细信息，请参阅[如何设置多功能设备或应用程序以使用 Microsoft 365 发送电子邮件](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。</span><span class="sxs-lookup"><span data-stu-id="a5545-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="a5545-104">如果你的设备或应用程序最近停止工作，最常见的问题有：</span><span class="sxs-lookup"><span data-stu-id="a5545-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="a5545-105">**使用 SMTP 身份验证客户端提交身份验证时出现的相关错误** 我们最近对 SMTP 身份验证的工作方式进行了一些更改。</span><span class="sxs-lookup"><span data-stu-id="a5545-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="a5545-106">有关如何解决问题的详细信息，请参阅[修复使用 Microsoft 365 或 Office 365 发送电子邮件的打印机、扫描仪和 LOB 应用程序的问题](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)的身份验证失败部分。</span><span class="sxs-lookup"><span data-stu-id="a5545-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="a5545-107">**我们只接受 TLS 1.2 版本，同时与 Office 365 建立安全连接** 如果你使用的是安全连接 (TLS)，请确保应用程序设备支持 TLS 1.2。</span><span class="sxs-lookup"><span data-stu-id="a5545-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="a5545-108">有关详细信息，请参阅[在 Office 365 和 Office 365 GCC 中准备 TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="a5545-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="a5545-109">有关其他问题和解决方案，请参阅[修复使用 Microsoft 365 或 Office 365 发送电子邮件的打印机、扫描仪和 LOB 应用程序的问题](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)。</span><span class="sxs-lookup"><span data-stu-id="a5545-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="a5545-110">要查看受影响的设备，请转到 [SMTP 身份验证客户端报表](https://protection.office.com/mailflow/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a5545-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="a5545-p103">**注意**：Exchange Online 不适用于批量邮件方案。若要发送批量商业电子邮件（例如，客户新闻稿），应使用专用于这些服务的第三方提供商。</span><span class="sxs-lookup"><span data-stu-id="a5545-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
