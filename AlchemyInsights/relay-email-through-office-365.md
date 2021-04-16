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
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809645"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="c7983-102">设置多功能设备或应用程序以发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="c7983-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="c7983-103">若要了解有关选项和步骤的详细信息，请参阅[如何设置多功能设备或应用程序以使用 Microsoft 365 发送电子邮件](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。</span><span class="sxs-lookup"><span data-stu-id="c7983-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="c7983-104">**注意：** 如果你的某设备或应用程序近期停止工作，请注意我们最近已开始按计划 [禁用 3DES 密码](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption)。</span><span class="sxs-lookup"><span data-stu-id="c7983-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="c7983-105">要查看受影响的设备，请转到 [SMTP 身份验证客户端报表](https://protection.office.com/mailflow/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="c7983-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="c7983-106">常见错误可能类似于：身份验证失败/错误、TLS 失败/错误、密码算法错误、算法不匹配或连接断开。</span><span class="sxs-lookup"><span data-stu-id="c7983-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="c7983-107">如何解决该问题：</span><span class="sxs-lookup"><span data-stu-id="c7983-107">To resolve the issue:</span></span>

 - <span data-ttu-id="c7983-108">**Windows Server 2003 IIS SMTP 将不再正常工作 – 需要更高版本的 Windows。**</span><span class="sxs-lookup"><span data-stu-id="c7983-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="c7983-109">请与你的应用程序或设备供应商核实，了解是否支持新式密码或是否有更新。</span><span class="sxs-lookup"><span data-stu-id="c7983-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
