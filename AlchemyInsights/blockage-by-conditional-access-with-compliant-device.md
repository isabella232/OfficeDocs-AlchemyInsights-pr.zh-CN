---
title: 由于使用符合条件的设备被条件访问阻止
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019138"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>由于使用符合条件的设备被条件访问阻止

**强烈建议使用的工具**

- [设备注册疑难解答](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) 工具 - 一种全面的工具，可帮助解决最常见的设备注册问题。
- [测试设备注册连接脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 一种用于确保设备可以访问系统帐户下的设备注册终结点的工具。
- [Azure AD 设备清理脚本](https://github.com/mzmaili/AzureADDeviceCleanup) - 一种用于查找和管理环境中过时的设备的工具。

以下是条件访问可能会失败（针对合规性设备）的一些常见原因，或者为什么用户可能会收到 **你在向组织资源登录请求期间收到** 邮件。

1. **设备不是 MDM 要求的设备状态**：

验证设备是否向批准的 MDM 提供商如 Intune 和 *标记为*。 有关 Intune 详细信息，请参阅此 [文档](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)。 若要更好地了解设备合规性和 Intune，请参阅 [合规性策略为通过 Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)管理的设备设置规则。 如果在使用 Intune 注册设备时遇到问题，请参阅 在 Microsoft [中解决设备注册问题并查找](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。 若要进一步获得 Intune 支持，请创建支持请求。 若要实现此点，请访问 [的 Intune 帮助和支持页面](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)。

2. **设备未加入组织网络**：

为访问组织资源，设备必须直接连接或虚拟专用网络 （VPN） 连接到组织的网络，并且还加入本地或 Azure Active Directory。 若要将工作设备加入组织网络，请参阅 [将工作设备加入组织的网络](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)。 要注册个人/BYOD 设备，请参阅 [组织网络共享设备上注册个人](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)。

- 若要验证设备是否已加入网络，可在[此处](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)工作设备[步骤](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)。 若要将问题的范围界定到组织网络连接，请按照以下准则操作：

    1. 使用工作或学校帐户（例如 alain@contoso.com）登录 Windows。
    2. 通过 VPN 或 DirectAccess 连接到组织的网络。
    3. 连接后，按 **Windows 徽标键+L** 锁定设备。
    4. 使用工作或学校帐户解锁设备，然后再次尝试访问有问题的应用和服务。

如果你看到错误消息 **无法从此处再次看到错误消息** ，则问题可能还有其他位置。

3. **不支持操作系统：**：

请确保正在运行的操作系统版本受支持，其中包括：

- **Windows 客户端**：Windows 7 或更高版本

- **Windows Server**：Windows Server 2008 R2 或更高版本

- **macOS**：macOS X 或更高版本

- **Android 和 iOS**：最新版本的 Android 和 iOS 移动操作系统

4. **不支持 Web 浏览器**：

请在下面找到支持的浏览器。 Chrome 支持 Windows 1703 或更高版本，需要 Windows 10 帐户扩展。 对于 Edge 85+，用户需要登录以正确传递设备合规性信息。 有关详细信息，请参阅 [此处](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)。

- **Windows 10**：Microsoft Edge、Internet Explorer、Chrome
- **Windows 8/8.1**：Internet Explorer、Chrome
- **Windows 7**：Internet Explorer、Chrome
- **iOS**：Microsoft Edge、Intune 托管浏览器、Safari
- **Android**： **Microsoft Edge**：Intune 托管浏览器，Chrome
- **Windows Phone**：Microsoft Edge、Internet Explorer
- **Windows Server 2019**：Microsoft Edge、Internet Explorer、Chrome
- **Windows Server 2016 更新**：Internet Explorer
- **Windows Server 2012 R2**：Internet Explorer
- **Windows Server 2008 R2**：Internet Explorer
- **macOS**：Chrome、Safari

在此处查找有关 **无法获取你的消息和疑难** 步骤 [此处](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)。
