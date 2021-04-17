---
title: 更改默认 Yammer 域
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817934"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>更改默认/主 Yammer 域

Yammer URL 包含 Yammer 网络的当前主域名。 此域名可能与 Office 365 或 Azure AD 中设置的主域名不匹配。 根据添加到租户的自定义域数目，以及 Yammer 是否在受支持的配置中（1 个租户：1 个网络，即 1:1），行为上存在差异。 提供了有关 [Yammer 域和 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) 的文档。

显示错误域的最常见原因是存在多个 Yammer 网络，需要进行合并。 使用网络迁移工具[向下整合到单个网络中](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)是至关重要的第一步。 完成此操作后，再尝试设置主域。

**无自定义域**

对于新租户，来自租户的默认域（例如 fabrikam.onmicrosoft.com）将用于 Yammer。 主域设置为 yammer.com/fabrikam.onmicrosoft.com。

**单个自定义域**

Yammer 将自动从租户中选择自定义域（例如 fabrikam.com）作为 Yammer 中的主域。 它设置为 yammer.com/fabrikam.com。 此更改是由域同步服务进行的，可能需要长达 24 小时才能生效。

**多个自定义域**

Yammer 可以拥有与默认租户域不同的主域。 由于存在多个自定义域，因此 Yammer 不会尝试猜测可用域中的正确域。 需要打开一个支持案例，请求将主域名改为所选的主域。

**其他疑难解答信息**

在某些情况下，租户之间可能移动了域，而域同步服务无法成功运行。 除了不正确的主域之外，可能还会遇到登录或其他问题。 若要解决此问题，你可能需要 Microsoft 支持部门的帮助将域移动到正确的网络。 这种情况需要直接协助，可能需要一些时间才能解决，特别是如果有一个很长的域名列表。 打开一个支持案例，以获取有关解决这些类型问题的帮助。

在与支持专员协作时，他们将检查是否已在你的控制之下的租户上验证域。 如果将域添加到你的租户但未通过 DNS 验证，他们可能会询问有关这些域的其他验证问题。 请确保 DNS 已对域进行验证，以便加快进程。
