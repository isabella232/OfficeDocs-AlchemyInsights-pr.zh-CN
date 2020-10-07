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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366418"
---
# <a name="monitoring-conditional-access-for-exchange"></a>监视对 Exchange 的条件访问

如果用户不符合组织的访问要求，则以条件访问为目标的用户将收到通知电子邮件。 若要解决此问题，我们建议采用以下一个或多个解决方案：

- 如果要注册设备，请建议用户转到公司门户应用程序，并验证它是否出现在公司门户中。 如果不是，则用户应注册该设备。
- 在 Azure 门户中，转到 Intune > 设备合规性。 在 "监视器单击" "设备符合性" 下。 查看设备合规性报告，以验证用户的设备是否已标记为合规。
- 在 Azure 门户中，转到 Intune > 设备合规性。 在 "管理" 下，单击 "策略"。 在合规性策略列表中，验证是否已将配置文件分配给您的用户设备。 如果未分配任何配置文件，则 Intune 将无法确认设备的符合性状态。
- 编辑用户的条件访问分配。

1. 在 Azure 门户中，转到**Intune**  >  **条件访问**  >  **策略**。
2. 从列表中选择一个策略。
3. 单击 "用户和组"。
4. 若要面向某人的特定策略，请将其添加到包含列表中。 若要确保从策略中忽略某个人，请将其添加到 "排除" 列表中。

帮助链接：

[设备合规性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[对 CA 进行故障排除](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[故障排除策略](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[监控 Intune 设备合规性](https://docs.microsoft.com/intune/compliance-policy-monitor)

注意：这些步骤仅有助于对 Azure Active Directory 功能条件访问进行故障排除。 此外，还可以通过 Exchange 策略隔离阻止其电子邮件访问的设备。 可在 [此处](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)找到有关 Exchange 设备管理的详细信息。
