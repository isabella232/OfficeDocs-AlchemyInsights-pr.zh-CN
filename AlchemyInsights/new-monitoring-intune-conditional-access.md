---
title: 监视 Intune 条件访问
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416983"
---
# <a name="monitor-intune-conditional-access"></a>监视 Intune 条件访问

如果条件访问的目标用户不符合组织的访问要求，他们将收到一封通知电子邮件。 若要解决，我们建议使用以下一个或多个解决方案：

1. 如果认为设备已注册，建议用户转到公司门户应用，并验证它是否显示在公司门户中。 如果没有，用户必须注册设备。
1. 在 Azure 门户中，转到 **Intune**  >  **设备合规性**。 
1. 若要查看设备合规性报告以验证用户设备是否标记为合规，请在 **"** 监视器"下，单击 **"设备合规性"。**
1. 在 Azure 门户中，转到 **Intune**  >  **设备合规性**。 在 **"管理"下**，单击 **"策略"。** 在合规性策略列表中，验证配置文件是否分配给用户设备。 如果未分配任何配置文件，则 Intune 将无法确认设备的合规性状态。
1. 编辑用户的条件访问分配。
1. 在 Azure 门户中，导航到 **Intune**  >  **条件访问**  >  **策略**，从列表中选择策略，然后单击"**用户和组"。**
1. 若要将特定策略面向某人，请将其添加到 **"包含"列表中**。 若要确保从策略中省略某人，请将其添加到排除 **列表中**。

**有用链接：**

- [设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)
- [CA 疑难解答](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [疑难解答策略](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [监视 Intune 设备合规性](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> 这些步骤仅有助于对 Azure Active Directory 功能条件访问进行疑难解答。 也可以隔离使用 Exchange 策略阻止其电子邮件访问的设备。 有关 Exchange 设备管理详细信息，请参阅 [**此处**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))。
