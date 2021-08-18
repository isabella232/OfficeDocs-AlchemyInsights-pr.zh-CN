---
title: 指示器使用 Edge 浏览器不起作用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326251"
---
# <a name="indicators-dont-work-using-edge-browser"></a>指示器使用 Edge 浏览器不起作用

创建指示器后，Edge （Smartscreen） 不授予其荣誉。 有关详细信息，请参阅 [IP 和 URL/域标记](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)。

## <a name="step-1-ensure-the-following"></a>步骤 1：确保以下内容

- 验证指示器是否正确（IP/URL 中无拼写错误，操作正确，RBAC 组正确）。
- 创建指示器后至少等待 2 小时，考虑任何可能延迟。
- 确认系统已载入 Microsoft Defender for Endpoint。
- 验证系统能否与云进行通信。
- 通过转到[测试站点](https://demo.smartscreen.msft.net)，验证Smartscreen是否已启用并可以访问。

## <a name="step-2-troubleshoot-the-potential-issue"></a>步骤 2：解决潜在问题

- 请确保客户端满足要求。 有关详细信息，请参阅 [创建 IP 和 URL/域指示器](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)。
- 请确保正在运行最新版本的 Edge 浏览器。 若要了解最新版本，请参阅 [了解你拥有哪个版本的 Microsoft Edge](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)。
- 重启 Edge 浏览器。
- 导航到已设置指示器的网站。 如果网站未按预期显示，请继续执行步骤 3。 

## <a name="step-3-collect-data"></a>步骤 3：收集数据

- 收集 **MDEClientAnalyzer** 诊断数据。 有关说明，请参阅 [将计算机载入到 Microsoft Defender for Endpoint](issues-with-onboarding-machines.md)。
- 如果你习惯安装和收集 Fiddler 跟踪，请参阅 [Telerik Fiddler](http://www.telerik.com/fiddler)。
- 如果希望从 Microsoft 支持人员获得指导，请选择下面的"支持"图标打开支持案例。
