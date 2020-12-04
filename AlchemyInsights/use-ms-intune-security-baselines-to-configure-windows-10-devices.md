---
title: 使用 Microsoft Intune 安全基准配置 Windows 10 设备
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571779"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="7cf38-102">使用 Microsoft Intune 安全基准配置 Windows 10 设备</span><span class="sxs-lookup"><span data-stu-id="7cf38-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="7cf38-103">Intune 安全基准可帮助保护用户和设备。</span><span class="sxs-lookup"><span data-stu-id="7cf38-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="7cf38-104">安全基准是 Windows 设置预配置的组，用于应用已知的设置组和相关安全团队建议的默认值。</span><span class="sxs-lookup"><span data-stu-id="7cf38-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="7cf38-105">通过在 Intune 中创建安全基准配置文件，可以创建一个包含多个设备配置配置文件的模板。</span><span class="sxs-lookup"><span data-stu-id="7cf38-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="7cf38-106">当您将安全基准部署到用户组或设备组时，这些设置将应用于在 Windows 10 或更高版本上运行的设备。</span><span class="sxs-lookup"><span data-stu-id="7cf38-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="7cf38-107">例如，MDM 安全基准自动 (1) 为可移动驱动器启用 BitLocker， (2) 需要用于解锁设备的密码， (3) 禁用基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="7cf38-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="7cf38-108">如果默认值不适用于您的环境，请自定义比较基准以应用所需的设置。</span><span class="sxs-lookup"><span data-stu-id="7cf38-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="7cf38-109">安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。</span><span class="sxs-lookup"><span data-stu-id="7cf38-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="7cf38-110">以下是一些优点：</span><span class="sxs-lookup"><span data-stu-id="7cf38-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="7cf38-111">安全基准包括影响安全性的设置的最佳实践和建议。</span><span class="sxs-lookup"><span data-stu-id="7cf38-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="7cf38-112">由于具有 Windows 安全团队的 Intune 合作伙伴创建组策略的基准，因此这些建议以坚实的指导和广泛的体验为依据。</span><span class="sxs-lookup"><span data-stu-id="7cf38-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="7cf38-113">如果你刚开始使用 Intune 并不确定从何处开始，安全基准将帮助你快速创建和部署安全配置文件。</span><span class="sxs-lookup"><span data-stu-id="7cf38-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="7cf38-114">如果你当前使用的是组策略，则将安全基准迁移到 Intune 以进行管理将更加简单，因为它们内置于 Intune 中，并包括用于管理的先进功能。</span><span class="sxs-lookup"><span data-stu-id="7cf38-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="7cf38-115">若要了解详细信息，请参阅 [Windows 安全基准](https://go.microsoft.com/fwlink/?linkid=2141503) 和 [移动设备管理](https://go.microsoft.com/fwlink/?linkid=2141701)。</span><span class="sxs-lookup"><span data-stu-id="7cf38-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>