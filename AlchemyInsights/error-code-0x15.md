---
title: 错误代码0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果在远程桌面服务（RDS）部署上激活 Office 2013 时收到错误，请考虑通过编辑注册表启用 ADAL。
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703128"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="cb540-103">在远程桌面服务上激活 Office 2013 时出现错误</span><span class="sxs-lookup"><span data-stu-id="cb540-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="cb540-104">如果在远程桌面服务（RDS）部署上激活 Office 2013 时收到错误，请考虑通过编辑注册表启用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="cb540-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="cb540-105">**注册表项**</span><span class="sxs-lookup"><span data-stu-id="cb540-105">**Registry key**</span></span>|<span data-ttu-id="cb540-106">**类型**</span><span class="sxs-lookup"><span data-stu-id="cb540-106">**Type**</span></span>|<span data-ttu-id="cb540-107">**值**</span><span class="sxs-lookup"><span data-stu-id="cb540-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cb540-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="cb540-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="cb540-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="cb540-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="cb540-110">1</span><span class="sxs-lookup"><span data-stu-id="cb540-110">1</span></span>  <br/> |

<span data-ttu-id="cb540-111">有关详细信息，请参阅[在 Windows 设备上为 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="cb540-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="cb540-112">默认情况下，在 Microsoft 365 应用程序的企业版和 Office 2016 中启用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="cb540-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="cb540-113">远程桌面服务（RDS）之前已被命名为 "终端服务"。</span><span class="sxs-lookup"><span data-stu-id="cb540-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  