---
title: 配置终结点 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: f29d8476881fb3f93b369c057efed0acdd2169baf956ab43bf3c0ade527e9437
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033520"
---
# <a name="configure-endpoint-dlp"></a>配置终结点 DLP

Microsoft Endpoint DLP 允许你将 DLP 保护和监视功能扩展至 Windows 10 设备上的敏感信息。 设备载入到设备管理后，你可以创建 DLP 策略，以便强制执行对项目的保护操作。 活动资源管理器可用于监视敏感项目的活动。 有关详细信息，请参阅 [将设备载入设备管理](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。  

开始使用终结点 DLP：

- 确保拥有相应的 SKU/订阅许可。 有关详细信息，请参阅 [SKU/订阅许可](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。
- 检查启用设备管理、访问载入页面或打开/关闭设备监视所需的权限。有关详细信息，请参阅 [权限](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。
- 按照载入设备步骤，将设备载入进设备管理。 有关详细信息，请参阅 [载入设备](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。 
- 创建 DLP 策略来保护你的敏感项目。 有关信息，请参阅[终结点 DLP 策略方案](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。

有关 Microsoft 终结点 DLP 的更多详细信息，请参阅 [了解 Microsoft 365 终结点数据丢失防护（预览版）](/microsoft-365/compliance/endpoint-dlp-learn-about)。

**如需要支持，请采取以下重要数据收集步骤：**

1. 下载 [MDATP 客户端分析器预览版](https://aka.ms/betamdatpanalyzer)。
1. 以管理员身份从 cmd 窗口运行该工具：

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. 当系统提示 **输入收集跟踪的分钟数：**，输入运行方案所需的分钟数。
1. 运行场景。

收集Zip文件输出以提供给支持代理。
