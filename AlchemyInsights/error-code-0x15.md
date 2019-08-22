---
title: 错误代码0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误, 请考虑通过编辑注册表启用 ADAL。
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526967"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>在远程桌面服务上激活 Office 2013 时出现错误

如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误, 请考虑通过编辑注册表启用 ADAL。
  
|**注册表项**|**Type**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

有关详细信息, 请参阅[在 Windows 设备上为 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  默认情况下, 在 Office 365 专业增强版和 Office 2016 中启用 ADAL。 远程桌面服务 (RDS) 之前已被命名为 "终端服务"。
  