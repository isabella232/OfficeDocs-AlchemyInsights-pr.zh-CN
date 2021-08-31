---
title: 登录应用Microsoft 365问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744622"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>登录 Microsoft 365 应用版

注意：如果你使用的是较旧版本的 Windows (例如 Windows 7 SP1、Windows Server 2008 R2) ，请使用简单修补程序启用 TLS 1.2 作为默认值。 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 有关详细信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

若要解决 Microsoft 365 应用的登录问题，请尝试在受影响的计算机上使用以下选项：  

- 有关Windows，请参阅推荐[解决常见登录问题](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- For Mac， see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**提示** 在 Windows 计算机上，我们可以为你诊断并自动修复若干常见的 Office 登录问题。 下载并运行 **[Microsoft 支持和恢复助手](https://aka.ms/SaRA-OfficeSignInScenario)** 以使用我们的自动化工具。

**注意：** 建议不要 (ADAL) 或 Web 帐户管理 (WAM) 修复登录或激活 **问题。** 如果使用 Microsoft 365 2013 连接到 Office 时发生错误，请确保为 Office 客户端启用新式[](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)验证。

有关特定的疑难解答操作，请参阅：

[Windows 10 上更新到 Office 2016 内部版本 16.0.7967 后登录时出现连接问题](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[你无法登录组织帐户，例如 Office 365、Azure 或 Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[如何排查无法登录 Azure、Azure 或 Intune Office 365浏览器应用的问题](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[反复提示输入Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)