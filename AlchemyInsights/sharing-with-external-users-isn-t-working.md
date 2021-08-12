---
title: 无法与外部用户共享
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910356"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>修复了SharePoint用户共享内容的问题

确保为组织启用外部共享：
  
1. 转到网站 [ &amp; 中的"服务"外接程序Microsoft 365 管理中心，然后单击](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)"网站 **"。**
    
2. 确保将设置设置为"开"。 如果选择了"仅现有外部用户"，请确保外部用户已列在Microsoft 365 管理中心。
    
确保为网站启用外部共享。 对于经典网站集：
  
1. 在管理中心SharePoint，单击左侧窗格中的"网站 **"。**
    
2. 选择一个或多个网站或网站，在功能区上单击"共享 **"。**
    
对于属于组或通信Microsoft 365团队网站：
  
- 这些新网站类型与组织范围的设置具有相同的共享设置，除非组织范围的设置允许使用不需要登录的链接共享文件。 在这种情况下，网站允许与登录的新外部用户和现有外部用户共享。 若要更改特定网站的设置，请使用新的 SharePoint 管理中心或 PowerShell。 [了解详细信息](https://go.microsoft.com/fwlink/?linkid=871863)。
    
> [!NOTE]
> 任何网站的外部共享设置可能比组织范围的设置更加严格，但与组织范围的设置的限制并不高。 
  

