---
title: SharePoint 中的 401 未授权错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539922"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="7fc47-102">SharePoint 中的 401 未授权错误</span><span class="sxs-lookup"><span data-stu-id="7fc47-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="7fc47-p101">如果在 SharePoint 中收到"（401） 未授权"错误，则它可能与 TLS 1.0/1.1 的弃用有关。有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="7fc47-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

- [<span data-ttu-id="7fc47-105">准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="7fc47-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="7fc47-106">如果客户端不支持 TLS 1.2，则会出现身份验证错误</span><span class="sxs-lookup"><span data-stu-id="7fc47-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="7fc47-107">更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议</span><span class="sxs-lookup"><span data-stu-id="7fc47-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="7fc47-108">如果用户使用 Windows 7，请确保他们查看 [Windows 7 中的 TLS 密码套件](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。</span><span class="sxs-lookup"><span data-stu-id="7fc47-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>