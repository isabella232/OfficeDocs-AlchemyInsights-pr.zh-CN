---
title: 错误代码0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误, 请考虑通过编辑注册表启用 ADAL。
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402729"
---
<span data-ttu-id="44dd7-103">如果在远程桌面服务 (RDS) 部署上激活 Office 2013 时收到错误, 请考虑通过编辑注册表启用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="44dd7-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="44dd7-104">**注册表项**</span><span class="sxs-lookup"><span data-stu-id="44dd7-104">**Registry key**</span></span>|<span data-ttu-id="44dd7-105">**类型**</span><span class="sxs-lookup"><span data-stu-id="44dd7-105">**Type**</span></span>|<span data-ttu-id="44dd7-106">**值**</span><span class="sxs-lookup"><span data-stu-id="44dd7-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="44dd7-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="44dd7-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="44dd7-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="44dd7-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="44dd7-109">1</span><span class="sxs-lookup"><span data-stu-id="44dd7-109">1</span></span>  <br/> |
   
<span data-ttu-id="44dd7-110">有关详细信息, 请参阅[在 Windows 设备上为 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="44dd7-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="44dd7-111">默认情况下, 在 office 365 专业增强版和 office 2016 中启用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="44dd7-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="44dd7-112">> 远程桌面服务 (RDS) 以前名为 "终端服务"。</span><span class="sxs-lookup"><span data-stu-id="44dd7-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

