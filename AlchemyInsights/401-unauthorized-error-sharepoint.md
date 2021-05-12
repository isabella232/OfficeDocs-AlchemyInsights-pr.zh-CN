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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233488"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="130bc-102">SharePoint 中的 401 未授权错误</span><span class="sxs-lookup"><span data-stu-id="130bc-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="130bc-p101">如果在 SharePoint 中收到"（401） 未授权"错误，则它可能与 TLS 1.0/1.1 的弃用有关。有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="130bc-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

[<span data-ttu-id="130bc-105">准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="130bc-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="130bc-106">如果客户端不支持 TLS 1.2，则会出现身份验证错误</span><span class="sxs-lookup"><span data-stu-id="130bc-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="130bc-107">如果用户使用 Windows 7，请确保他们查看 [Windows 7 中的 TLS 密码套件](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。</span><span class="sxs-lookup"><span data-stu-id="130bc-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>