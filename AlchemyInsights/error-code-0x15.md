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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277479"
---
<span data-ttu-id="cd07d-103">如果您正在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误消息，请考虑启用 ADAL 通过编辑注册表。</span><span class="sxs-lookup"><span data-stu-id="cd07d-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="cd07d-104">**注册表项**</span><span class="sxs-lookup"><span data-stu-id="cd07d-104">**Registry key**</span></span>|<span data-ttu-id="cd07d-105">**类型**</span><span class="sxs-lookup"><span data-stu-id="cd07d-105">**Type**</span></span>|<span data-ttu-id="cd07d-106">**值**</span><span class="sxs-lookup"><span data-stu-id="cd07d-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cd07d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="cd07d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="cd07d-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="cd07d-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="cd07d-109">1</span><span class="sxs-lookup"><span data-stu-id="cd07d-109">1</span></span>  <br/> |
   
<span data-ttu-id="cd07d-110">有关详细信息，请参阅[Office 2013 的 Windows 设备启用现代身份验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="cd07d-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="cd07d-p101">默认情况下，在 Office 365 ProPlus 和 Office 2016 启用 ADAL。> 远程桌面服务 (RDS) 主题以前名为终端服务。</span><span class="sxs-lookup"><span data-stu-id="cd07d-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

