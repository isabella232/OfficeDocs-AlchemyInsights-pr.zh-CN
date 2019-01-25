---
title: 错误代码 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您正在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误消息，请考虑启用 ADAL 通过编辑注册表。
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499372"
---
如果您正在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误消息，请考虑启用 ADAL 通过编辑注册表。 
  
|**注册表项**|**类型**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |^1  <br/> |
   
有关详细信息，请参阅[Office 2013 的 Windows 设备启用现代身份验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  默认情况下，在 Office 365 ProPlus 和 Office 2016 启用 ADAL。> 远程桌面服务 (RDS) 主题以前名为终端服务。 
  

