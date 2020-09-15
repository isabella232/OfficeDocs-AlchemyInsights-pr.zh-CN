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
description: 如果在远程桌面服务上激活 Office 2013 时收到错误 (RDS) 部署，请考虑通过编辑注册表启用 ADAL。
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709177"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>在远程桌面服务上激活 Office 2013 时出现错误

如果在远程桌面服务上激活 Office 2013 时收到错误 (RDS) 部署，请考虑通过编辑注册表启用 ADAL。
  
|**注册表项**|**类型**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

有关详细信息，请参阅 [在 Windows 设备上为 Office 2013 启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  默认情况下，在 Microsoft 365 应用程序的企业版和 Office 2016 中启用 ADAL。 之前已将 (RDS) 的远程桌面服务命名为 "终端服务"。
  