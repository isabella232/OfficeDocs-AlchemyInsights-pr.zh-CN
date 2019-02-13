---
title: 错误代码 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您正在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误消息，请考虑启用 ADAL 通过编辑注册表。
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929078"
---
如果您正在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误消息，请考虑启用 ADAL 通过编辑注册表。 
  
|**注册表项**|**类型**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
有关详细信息，请参阅[Office 2013 的 Windows 设备启用现代身份验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  默认情况下，在 Office 365 ProPlus 和 Office 2016 启用 ADAL。> 远程桌面服务 (RDS) 主题以前名为终端服务。 
  

