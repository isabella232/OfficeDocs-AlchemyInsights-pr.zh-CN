---
title: Intune Win32 应用部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366495"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="4bea4-102">Intune Win32 应用部署</span><span class="sxs-lookup"><span data-stu-id="4bea4-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="4bea4-103">Microsoft Intune 允许 Win32 应用程序（包括但不限于 MSI 和 .EXE ）部署到 Windows 10 设备。</span><span class="sxs-lookup"><span data-stu-id="4bea4-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="4bea4-104">使用的部署机制要求目标设备上存在 Intune 管理扩展 (IME)。</span><span class="sxs-lookup"><span data-stu-id="4bea4-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="4bea4-105">将 powershell 脚本或 win32 应用程序部署定向到用户/设备后，将自动安装 IME。</span><span class="sxs-lookup"><span data-stu-id="4bea4-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="4bea4-106">还必须满足一组先决条件才能部署 Win32 应用，其中包括：</span><span class="sxs-lookup"><span data-stu-id="4bea4-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="4bea4-107">支持的平台：Windows 10 版本 1607 或更高版本（企业版、专业版和教育版）。</span><span class="sxs-lookup"><span data-stu-id="4bea4-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="4bea4-108">支持的体系结构：x86 和 x64。</span><span class="sxs-lookup"><span data-stu-id="4bea4-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="4bea4-109">设备管理：已加入 AAD 和自动注册（包括已加入混合域和自动注册组策略）。</span><span class="sxs-lookup"><span data-stu-id="4bea4-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="4bea4-110">应用程序包格式：由 [Microsoft Win32 内容准备工具](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)准备的 .**intunewin** 文件。</span><span class="sxs-lookup"><span data-stu-id="4bea4-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="4bea4-111">限制：</span><span class="sxs-lookup"><span data-stu-id="4bea4-111">Limitations:</span></span>
    - <span data-ttu-id="4bea4-112">最大大小：8GB。</span><span class="sxs-lookup"><span data-stu-id="4bea4-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="4bea4-113">不支持的体系结构：ARMs。</span><span class="sxs-lookup"><span data-stu-id="4bea4-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="4bea4-114">有关这些步骤的相关信息，请查看文档“[在 Microsoft Intune 中添加、分配和监控 Win32 应用](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)”。</span><span class="sxs-lookup"><span data-stu-id="4bea4-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="4bea4-115">有关在 Windows 上对应用程序部署（包括 Win32 应用）进行故障排除的详细信息，请参阅以下文档</span><span class="sxs-lookup"><span data-stu-id="4bea4-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="4bea4-116">应用安装问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="4bea4-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="4bea4-117">Win32 应用疑难解答</span><span class="sxs-lookup"><span data-stu-id="4bea4-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)