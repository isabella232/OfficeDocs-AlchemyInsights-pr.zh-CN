---
title: 监视条件访问
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713708"
---
# <a name="monitoring-conditional-access-for-exchange"></a>监视对 Exchange 的条件访问

如果用户不符合组织的访问要求，则以条件访问为目标的用户将收到通知电子邮件。 若要解决此问题，我们建议采用以下一个或多个解决方案：
  
- 如果要注册设备，请建议用户转到公司门户应用程序，并验证它是否出现在公司门户中。 如果不是，则用户应注册该设备。
    
- 在 Azure 门户中，转**到\> Intune 设备符合性**。 在 "**监视器**单击" "**设备符合性**" 下。 查看设备合规性报告，以验证用户的设备是否已标记为合规。 
    
- 在 Azure 门户中，转**到\> Intune 设备符合性**。 在 "**管理**" 下，单击 "**策略**"。 在合规性策略列表中，验证是否已将配置文件分配给您的用户设备。 如果未分配任何配置文件，则 Intune 将无法确认设备的符合性状态。 
    
- 编辑用户的条件访问分配。
    
1. 在 Azure 门户中，转**到\> Intune 条件\>访问策略**
    
2. 从列表中选择策略
    
3. 单击 "**用户和组**"
    
4. 若要面向某人的特定策略，请将其添加到**包含**列表中。 若要确保从策略中忽略某个人，请将其添加到 "**排除**" 列表中。 
    
阅读详细信息：[如何监视条件访问设备](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

