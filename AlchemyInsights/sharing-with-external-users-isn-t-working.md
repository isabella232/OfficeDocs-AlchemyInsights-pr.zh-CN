---
title: 与外部用户共享不起作用
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747588"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>解决与外部用户共享 SharePoint 内容的问题

确保为您的组织打开了外部共享:
  
1. 转到[Microsoft 365 &amp;管理中心中的 "服务外接程序" 页](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), 然后单击 "**网站**"。
    
2. 确保设置为 "打开"。 如果选择 "仅现有的外部用户", 请确保外部用户在 Microsoft 365 管理中心中列出。
    
请确保为网站打开了外部共享。 对于经典网站集:
  
1. 在新的 SharePoint 管理中心中, 在左侧窗格中, 单击 "**网站**"。
    
2. 选择一个或一网站, 然后在功能区上, 单击 "**共享**"。
    
对于属于 Office 365 组或通信网站的团队网站:
  
- 这些新网站类型的共享设置与组织范围的设置相同, 除非组织范围设置允许使用不需要登录的链接共享文件。 在这种情况下, 网站允许与登录的新的和现有的外部用户共享。 若要更改特定网站的设置, 请使用新的 SharePoint 管理中心或 PowerShell。 [了解详细信息](https://go.microsoft.com/fwlink/?linkid=871863)。
    
> [!NOTE]
> 任何网站的外部共享设置的限制可能高于组织范围的设置, 但比组织范围设置更许可。 
  

