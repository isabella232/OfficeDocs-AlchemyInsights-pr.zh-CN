---
title: EndPoint Manager - 安全基准
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440866"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - 安全基准

安全基准是预配置的 Windows 设置组，可帮助应用相关安全团队推荐的安全设置。 这些比较基准可以自定义，以仅提供所需的设置和值。 有关安全基线详细信息，请参阅使用 [在 Intune 设备中配置 Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)。

这些产品当前有比较基准：

- Windows MDM 安全设置
- 适用于 EndPoint 安全性的 Microsoft Defender
- Microsoft Edge

每个基准会定期更新，并按增量版本发布。 每个版本都会添加或删除早期版本中的设置，以确保基线满足当前指导。 终结点安全中的安全基线控制台通过显示版本更改来比较不同版本。

有关如何最有效地更改所部署的基线版本的指导，请参阅 [Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)。

部署安全基准后，可监视部署状态并按设备查看设置。

**注意：** 基准的报告数据可能需要多达 24 小时才能从初始部署显示到设备，而进一步更新最多需要 6 小时。 

基线设置不应用最常见的原因是在不同的配置文件中使用的设置相同。 可通过从"安全基线"配置文件的"设备状态"节点中选择特定设备来调查此方案。 有关详细信息，请参阅 [解决安全基线](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)。