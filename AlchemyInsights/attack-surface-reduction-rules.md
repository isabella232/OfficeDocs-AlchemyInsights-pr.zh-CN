---
title: 攻击面减少规则
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
- "11228"
- "9005470"
ms.openlocfilehash: 1eb0d949693916d1192fb75132207cd6a52e75840899e57c089a5f5aaca3ca88
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893125"
---
# <a name="attack-surface-reduction-rules"></a>攻击面减少规则

排除文件或文件夹可以严重削弱攻击面减少规则提供的保护。 允许本将由规则阻止的文件运行，并且不会记录任何报告或事件。 排除应用于允许排除的所有规则。

ASR 排除使用与 Microsoft Defender 防病毒排除相同的语法。 有关详细信息，请参阅 [配置和验证 Microsoft Defender 防病毒扫描的排除](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)。 若要避免问题，请查看 [定义排除时要避免的常见错误](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)。

并非所有 ASR 规则都支持排除。 要验证规则是否支持排除，请参阅表 [攻击面减少规则](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)。

## <a name="attack-surface-reduction-rules"></a>攻击面减少规则

组织攻击面包括攻击者可能攻击组织设备或网络的所有位置。 减少攻击面意味着保护组织设备和网络，减少攻击者执行攻击的方式。 在 Microsoft Defender for Endpoint 中配置攻击面减少规则会有助于此。

有关详细信息，请参阅：

- [将 ASR 规则 GUID 映射到名称](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR 规则要求：
    - [Windows 10 专业版，版本 1709 或更高版本](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 企业版，版本 1709 或更高版本](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server 版本 1803（半年度频道）或更高版本](https://docs.microsoft.com/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>识别正确排除以应用

1. 在 Microsoft-Windows-Windows Defender/Operational.log 中查找 eventID 1121 或 1122。

1. 评估此方案需要取消阻止的阻止方案和上下文。

1. 读取事件详细信息中的路径值，即定义该排除的值。
    - 尽可能严格地进行排除。
    - 按需应用通配符（例如替换用户变量）。

1. 根据部署需求应用排除。 有关详细信息，请参阅 [自定义攻击面减少规则](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)。

## <a name="exclusion-is-not-honored"></a>不尊重排除

1. 确定规则是否支持排除。 有关详细信息，请参阅 [自定义减少攻击面规则](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)。

1. 查看已应用的排除，并通过事件数据验证键入错误或解读错误的通配符。 有关详细信息，请参阅 [支持的排除类型](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. 如果规则影响过大，请考虑将规则移动（或移回）到审核模式，以执行进一步验证。 有关详细信息，请参阅 [测试 Microsoft Defender for Endpoint 功能在审核模式下的工作情况](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/audit-windows-defender)。

1. 通过使用此命令收集支持数据，以打开支持案例：
    
   ** MDEClientAnalyzer.cmd -v**

    有关详细信息，请参阅 [将计算机载入到 Microsoft Defender for Endpoint 时出现问题](issues-with-onboarding-machines.md)。
