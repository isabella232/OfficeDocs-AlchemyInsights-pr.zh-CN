---
title: 监控条件的访问
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278064"
---
# <a name="monitoring-conditional-access"></a>监控条件的访问

目标具有条件的访问权限的用户将收到通知电子邮件，如果他们不能满足您组织的访问要求。若要解决，我们建议一个或多个以下解决方案：
  
- 如果设备则假定为注册，告知用户转到的公司门户应用程序并验证是否显示在公司门户。如果没有，用户应注册设备。
    
- 在 Azure 门户中，转到**Intune\>设备合规性**。在**监视**下单击**设备合规性**。查看您的设备合规性报告，以验证用户的设备已标记为兼容。 
    
- 在 Azure 门户中，转到**Intune\>设备合规性**。在**管理**下单击**策略**。在合规性策略列表中，验证该配置文件分配给用户的设备。如果没有分配配置，然后 Intune 将不能以确认设备的合规性状态。 
    
- 编辑用户的条件访问分配。
    
1. 在 Azure 门户中，转到**Intune\>条件访问\>策略**
    
2. 从列表中选择一个策略
    
3. 单击**用户和组**
    
4. 针对特定的策略某人时，将其添加到**包括**列表。若要确保人员省略从策略，请将其添加到**排除**列表中。 
    
阅读其他信息：[如何监视条件访问设备](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

