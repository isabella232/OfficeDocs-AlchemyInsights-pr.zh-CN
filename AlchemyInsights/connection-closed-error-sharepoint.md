---
title: SharePoint 中的基础连接已关闭错误
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044402"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>SharePoint 中的"基础连接已关闭"错误

如果你在 SharePoint 中收到"基础连接已关闭"的错误，它可能与 TLS 1.0/1.1 的弃用有关。有关详细信息，请参阅以下文章：

- [准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [如果客户端不支持 TLS 1.2，则会出现身份验证错误](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

如果用户使用 Windows 7，请确保他们查看 [Windows 7 中的 TLS 密码套件](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。