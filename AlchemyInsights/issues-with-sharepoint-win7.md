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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Windows 7 计算机上的 SharePoint 问题

如果在使用 SharePoint 或 OneDrive 时在 Windows 7 计算机上收到错误，则这些错误可能与 TLS 1.0/1.1 的弃用有关。 有关详细信息，请参阅：

- [准备在 Office 365 和 Office 365 GCC 中使用 TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 客户端必须启用 TLS1.2。 有关详细信息，请参阅[客户端不支持 TLS 1.2 时，出现身份验证错误](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- 安装 KB3140245 并创建注册表值。 有关更多信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windows 7 SP1/Windows 8 客户端必须确保安装了最新的 TLS 密码套件。 有关详细信息，请参阅 [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)。 


