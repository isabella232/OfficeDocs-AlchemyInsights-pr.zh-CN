---
title: 错误代码0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误，请考虑通过编辑注册表启用 ADAL。
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100752"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>在远程桌面服务Office 2013 激活时出错

如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误，请考虑通过编辑注册表启用 ADAL。
  
|**注册表项**|**类型**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

有关详细信息，请参阅在 Windows 设备上为[Office 2013 启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  ADAL 在 2016 年 Microsoft 365 企业应用版 Office默认启用。 RDS (远程桌面) 以前称为终端服务。
  