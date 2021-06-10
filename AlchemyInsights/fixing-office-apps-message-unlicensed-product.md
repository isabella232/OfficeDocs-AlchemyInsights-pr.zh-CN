---
title: 无法激活 Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798670"
---
# <a name="unable-to-activate-office"></a>无法激活 Office

**注意**：如果正在使用较早版本的 Windows（例如 Windows 7），请确保启用 TLS 1.2 为默认值。 有关详细信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

- 检查你的订阅状态是否已过期。
- 请确保你拥有允许客户端许可证的订阅（如 Office 365 商业版或商业高级版），并[确保该用户分配有许可证](/microsoft-365/admin/manage/assign-licenses-to-users)。
- 确保用户使用分配有许可证的同一帐户登录到 Office。
- 查看 [Office 365 服务运行状况页面](/office365/enterprise/view-service-health)，检查是否存在任何已知的服务问题。
- 检查防火墙、防病毒软件和代理设置，确认它们并未阻止 Microsoft 365 应用访问 Internet。请参阅 [Office 365 URL 和 IP 地址范围](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 和 IP 地址范围")。

**提示** 在 Windows 计算机上，我们可以为你诊断并自动修复若干常见的 Office 登录问题。 下载并运行 **[Microsoft 支持和恢复助手](https://aka.ms/SaRA-OfficeSignInScenario)** 以使用我们的自动化工具。

采取下列故障排除操作：

- 打开 Office 应用，然后[注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有用户帐户。 [移除](/microsoft-365/admin/manage/remove-licenses-from-users)并[重新分配](/microsoft-365/admin/manage/assign-licenses-to-users) Office 许可证，然后使用受影响的用户帐户[登录 Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。
- 运行[激活故障排除程序](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [重置 Office 激活状态](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "重置 Office 激活状态")
- [执行 Office 的联机修复](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

有关其他故障排除解决方案，请参阅：  

- [Office 中未经授权产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [激活 Office 时出现错误“很抱歉，无法连接到你的帐户。请稍后重试”](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)