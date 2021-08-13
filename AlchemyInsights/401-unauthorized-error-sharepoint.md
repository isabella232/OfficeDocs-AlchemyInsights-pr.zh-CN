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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919017"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>SharePoint 中的 401 未授权错误

如果在 SharePoint 中收到"（401） 未授权"错误，则它可能与 TLS 1.0/1.1 的弃用有关。有关详细信息，请参阅：

- [准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [如果客户端不支持 TLS 1.2，则会出现身份验证错误](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

如果用户使用 Windows 7，请确保他们查看 [Windows 7 中的 TLS 密码套件](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。