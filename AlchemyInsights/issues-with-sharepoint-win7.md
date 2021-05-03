---
title: Windows 7 计算机上的 SharePoint 问题
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066986"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="a019a-102">Windows 7 计算机上的 SharePoint 问题</span><span class="sxs-lookup"><span data-stu-id="a019a-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="a019a-103">如果在使用 SharePoint 或 OneDrive 时在 Windows 7 计算机上收到错误，则这些错误可能与 TLS 1.0/1.1 的弃用有关。</span><span class="sxs-lookup"><span data-stu-id="a019a-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="a019a-104">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a019a-104">For more information, see:</span></span>

- [<span data-ttu-id="a019a-105">准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="a019a-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="a019a-106">Windows 7 SP1/Windows 8 客户端必须启用 TLS1.2。</span><span class="sxs-lookup"><span data-stu-id="a019a-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="a019a-107">有关详细信息，请参阅[客户端不支持 TLS 1.2 时，出现身份验证错误](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="a019a-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="a019a-108">安装 KB3140245 并创建注册表值。</span><span class="sxs-lookup"><span data-stu-id="a019a-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="a019a-109">有关更多信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="a019a-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="a019a-110">Windows 7 SP1/Windows 8 客户端必须确保安装了最新的 TLS 密码套件。</span><span class="sxs-lookup"><span data-stu-id="a019a-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="a019a-111">有关详细信息，请参阅 [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)。</span><span class="sxs-lookup"><span data-stu-id="a019a-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


