---
title: 监视条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975091"
---
# <a name="monitoring-conditional-access-for-exchange"></a>监视条件访问Exchange

如果具有条件访问的用户不符合组织的访问要求，他们将收到一封通知电子邮件。 若要解决，我们建议使用下列一个或多个解决方案：

- 如果认为设备已注册，请建议公司门户应用并验证设备是否公司门户。 如果没有，则用户应注册设备。
- 在 Azure 门户中，转到 Intune >设备合规性。 在"监视器"下，单击"设备合规性"。 查看设备合规性报告，验证用户设备是否标记为合规。
- 在 Azure 门户中，转到 Intune >设备合规性。 在"管理"下，单击"策略"。 在合规性策略列表中，验证配置文件是否分配给用户设备。 如果未分配任何配置文件，则 Intune 将无法确认设备的合规性状态。
- 编辑用户的条件访问分配。

1. 在 Azure 门户中，转到 **Intune**  >  **条件访问**  >  **策略**。
2. 从列表中选择策略。
3. 单击"用户和组"。
4. 若要将特定策略面向某人，请将其添加到"包含"列表。 若要确保从策略中省略某人，请将其添加到排除列表中。

有用链接：

[设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 疑难解答](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[疑难解答策略](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[监视 Intune 设备合规性](https://docs.microsoft.com/intune/compliance-policy-monitor)

注意：这些步骤仅有助于对功能条件访问Azure Active Directory疑难解答。 也可以隔离使用策略阻止其电子邮件访问Exchange。 有关设备Exchange详细信息，请参阅 [此处 https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) ] (。
