---
title: 使用Microsoft Intune安全基线配置Windows 10设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783166"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="a99ec-102">使用Microsoft Intune安全基线配置Windows 10设备</span><span class="sxs-lookup"><span data-stu-id="a99ec-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="a99ec-103">Intune 安全基准可帮助保护用户和设备。</span><span class="sxs-lookup"><span data-stu-id="a99ec-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="a99ec-104">安全基线Windows设置预配置的组，用于应用相关安全团队建议的已知设置组和默认值。</span><span class="sxs-lookup"><span data-stu-id="a99ec-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="a99ec-105">在 Intune 中创建安全基线配置文件，可创建包含多个设备配置文件的模板。</span><span class="sxs-lookup"><span data-stu-id="a99ec-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="a99ec-106">将安全基线部署到用户组或设备组时，这些设置将应用于在 Windows 10 或更高版本运行的设备。</span><span class="sxs-lookup"><span data-stu-id="a99ec-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="a99ec-107">例如，Microsoft 移动设备管理 (MDM) 安全基线自动为可移动驱动器启用 BitLocker、需要用于解锁设备的密码以及禁用基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="a99ec-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="a99ec-108">当默认值对环境不起作用时，您可以自定义比较基准，以应用所需的设置。</span><span class="sxs-lookup"><span data-stu-id="a99ec-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="a99ec-109">安全基准还有助于在 Microsoft 365 中建立端到端的安全工作流。</span><span class="sxs-lookup"><span data-stu-id="a99ec-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="a99ec-110">安全基准包括影响安全性的设置最佳做法和建议。</span><span class="sxs-lookup"><span data-stu-id="a99ec-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="a99ec-111">Intune 合作伙伴与Windows团队合作，为组策略创建基线，因此这些建议基于可靠指导和广泛的经验。</span><span class="sxs-lookup"><span data-stu-id="a99ec-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="a99ec-112">如果你是 Intune 的新增用户，并且不确定从何处开始，安全基线可帮助你快速创建和部署安全配置文件。</span><span class="sxs-lookup"><span data-stu-id="a99ec-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="a99ec-113">如果当前使用组策略，则迁移到 Intune 以用于管理目的会更加轻松使用安全基线，因为它们内置于 Intune 中，并且包括最边缘的管理功能。</span><span class="sxs-lookup"><span data-stu-id="a99ec-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="a99ec-114">若要了解更多信息，请参阅Windows[基线和](/windows/security/threat-protection/windows-security-baselines)[移动设备管理](/windows/client-management/mdm/)。</span><span class="sxs-lookup"><span data-stu-id="a99ec-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

