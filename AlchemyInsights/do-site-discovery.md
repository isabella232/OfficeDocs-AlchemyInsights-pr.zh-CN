---
title: 进行站点发现
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529192"
---
# <a name="do-site-discovery"></a>进行站点发现

如果你的组织仍在使用旧版 Web 应用程序和计划以使用 Internet Explorer 模式（大多数客户都采用此模式），则你应该执行一些附加网站发现。

**你已部署早期版本的 Microsoft Edge**

如果你已配置你的企业网站列表以适用于旧版本的 Microsoft Edge，则你的网站发现将几乎完成。 你可能需要做的一件事是添加非特定语言的网站。

中性站点通常是提供单一登录 (SSO) 的站点。 如果从 Microsoft Edge 中导航到中性站点，则需要保持在 Microsoft Edge 中以进行身份验证。 如果在 Internet Explorer 模式下导航到中性站点，则需要保持在 Internet Explorer 模式中以进行身份验证。

标识使用的任何 SSO（或其他中性）站点，并将它们添加到企业站点列表中。

**Internet Explorer 是默认浏览器**

如果当前仅使用 Internet Explorer，则可能不知道哪些站点已升级到新式 Web 标准，以及哪些仍需要 Internet Explorer。 你需要查找这些网站并将其添加到企业网站列表，以便只为这些站点使用 Internet Explorer 模式。

> [!NOTE]
> [企业网站发现](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) 发现可能需要 Internet Explorer 模式的网站。 它可以在通过 Windows 10、Windows 8.1 或 Windows 7 上的 Internet Explorer 11 运行 Windows Internet Explorer 8 的计算机上收集数据。

**分析数据**

收集站点数据后，我们建议采用以下 4 步过程来分析数据：
1. 依次按域和 URL 对数据进行排序。
2. 定义要为 Internet Explorer 模式配置的“应用”的边界。 您希望包含定义应用的所有网站和 Web 控件，但不想包含额外的网站和控件。 某些网站可能很简单，*https://contoso.com/app1* 而其他网站可能需要你定义多个网站和页面。
3. 测试应用以验证它是否未在本机工作。 许多站点在检测到新式浏览器时将提供新式内容，并且仅在检测到 Internet Explorer 时才提供旧版内容。
4. 如果应用未通过测试，请将该应用添加到企业站点列表中。

> [!NOTE]
> 作为最佳做法，请将构成应用的所有站点归为一组。 这样，当升级应用时，可以更轻松地从 Internet Explorer 模式中删除整个站点并开始将新式浏览器用于该应用。

完成网站发现并分析数据后，即可开始查看频道策略。

