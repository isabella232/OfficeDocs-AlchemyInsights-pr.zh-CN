---
title: 与外部用户共享不能正常工作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459324"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>修复与外部用户共享 SharePoint 内容的问题

请确保您的组织外部共享已打开：
  
1. 转到[服务&amp;加载项在 Office 365 管理中心页](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，并单击**站点**。
    
2. 请确保设置已打开到"开"。如果"仅现有的外部用户"处于选中状态，请确保外部用户是否列在 Office 365 管理中心。
    
请确保外部共享其开启网站。为经典网站集：
  
1. 在经典 SharePoint 管理中心，在左侧窗格中，单击**网站集**。
    
2. 选择或多个站点，然后在功能区上单击**共享**。
    
对于属于 Office 365 组中，工作组网站或通信网站：
  
- 这些新的网站类型具有相同共享设置为您的组织范围的设置，除非组织范围的设置允许共享使用的不需要登录链接的文件。在这种情况下，网站允许与新的和现有登录的外部用户共享。若要更改为特定站点的设置，使用新的 SharePoint 管理员中心 （预览） 或 PowerShell。[了解更多](https://go.microsoft.com/fwlink/?linkid=871863)。
    
> [!NOTE]
> 可以比您组织范围的设置，但不是更 permissive 比组织范围内设置更严格的任何网站的外部共享设置。 
  

