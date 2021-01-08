---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778183"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="27711-102">使用 Intune 启用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="27711-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="27711-103">Intune Endpoint Protection 策略可用于为 Windows 设备配置 Bitlocker 加密设置。</span><span class="sxs-lookup"><span data-stu-id="27711-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="27711-104">有关详细信息，请参阅 Windows 10 (及更高版本) [Intune 保护设备。](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="27711-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="27711-105">除了终结点保护策略之外，还有一个加密报告，它提供设备的加密状态的更详细视图。</span><span class="sxs-lookup"><span data-stu-id="27711-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="27711-106">此报告可以从 MEM 门户在"设备监控 **>"** 下访问，然后在"配置选择加密"[报告下访问](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)。</span><span class="sxs-lookup"><span data-stu-id="27711-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="27711-107">如果发现 Bitlocker 无法按预期启用，或者用于启用 Bitlocker 的配置文件的状态错误，请查看加密报告，以便更好地了解发生此行为的原因。</span><span class="sxs-lookup"><span data-stu-id="27711-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="27711-108">若要查找有关如何解释报告的详细信息，包括各种加密状态值，请参阅使用 [Intune 监视设备加密](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)。</span><span class="sxs-lookup"><span data-stu-id="27711-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="27711-109">你应该知道，许多运行 Windows 10 的较新设备都支持自动 Bitlocker 加密，无需应用 MDM 策略即可触发。</span><span class="sxs-lookup"><span data-stu-id="27711-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="27711-110">如果配置了非默认设置，这可能会影响策略的应用。</span><span class="sxs-lookup"><span data-stu-id="27711-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="27711-111">有关详细信息，请参阅以下常见问题解答。</span><span class="sxs-lookup"><span data-stu-id="27711-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="27711-112">有关 bitlocker 问题疑难解答的信息，请参阅 Microsoft Intune 中的 [BitLocker](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)策略疑难解答。</span><span class="sxs-lookup"><span data-stu-id="27711-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="27711-113">**常见问题解答**</span><span class="sxs-lookup"><span data-stu-id="27711-113">**FAQ**</span></span>

<span data-ttu-id="27711-114">问：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？</span><span class="sxs-lookup"><span data-stu-id="27711-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="27711-115">答：Intune Endpoint Protection 策略中的设置是使用 [Bitlocker CSP 实现的](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)。</span><span class="sxs-lookup"><span data-stu-id="27711-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="27711-116">并非所有版本的 Windows 都支持 Bitlocker CSP。</span><span class="sxs-lookup"><span data-stu-id="27711-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="27711-117">问：如何在无需最终用户交互的情况下在设备上启用 Bitlocker？</span><span class="sxs-lookup"><span data-stu-id="27711-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="27711-118">答：只要满足必要的先决条件，就可以通过 Intune 启用 Bitlocker"无提示加密"。</span><span class="sxs-lookup"><span data-stu-id="27711-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="27711-119">请参阅以下文档中的设备要求和示例策略设置的详细信息，以启用无提示加密：无提示 [启用 Bitlocker 加密](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)。</span><span class="sxs-lookup"><span data-stu-id="27711-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="27711-120">问：如果设备已使用适用于加密方法和加密强度 (XTS-AES-128) 的操作系统默认设置使用 Bitlocker 进行加密，那么应用不同设置的策略是否将自动触发使用新设置的驱动器重新加密？</span><span class="sxs-lookup"><span data-stu-id="27711-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="27711-121">答：不可以。</span><span class="sxs-lookup"><span data-stu-id="27711-121">A: No.</span></span> <span data-ttu-id="27711-122">若要应用新的密码设置，必须先解密驱动器。</span><span class="sxs-lookup"><span data-stu-id="27711-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="27711-123">**注意：** 对于使用 Autopilot 注册的设备，在评估 Intune 策略之前，不会触发在 OOBE 期间发生的自动加密，这将允许使用基于策略的设置来更改操作系统默认值。</span><span class="sxs-lookup"><span data-stu-id="27711-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="27711-124">问：如果设备由于 Intune 策略的应用而加密，那么在删除该策略时，设备是否将被解密？</span><span class="sxs-lookup"><span data-stu-id="27711-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="27711-125">答：删除与加密相关的策略不会解密已配置的驱动器。</span><span class="sxs-lookup"><span data-stu-id="27711-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="27711-126">问：为什么 Intune 合规性策略显示我的设备未启用 Bitlocker，即使它已启用？</span><span class="sxs-lookup"><span data-stu-id="27711-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="27711-127">答：Intune 合规性策略中的"启用 Bitlocker"设置利用 Windows 设备运行状况证明 (DHA) 客户端。</span><span class="sxs-lookup"><span data-stu-id="27711-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="27711-128">此客户端仅在启动时测量设备状态。</span><span class="sxs-lookup"><span data-stu-id="27711-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="27711-129">因此，如果自 Bitlocker 加密完成后设备尚未重新启动，DHA 客户端服务将不会报告 Bitlocker 处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="27711-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 