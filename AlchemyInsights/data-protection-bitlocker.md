---
title: DataProtection-Bitlocker
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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731229"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="51389-102">使用 Intune 启用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="51389-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="51389-103">Intune Endpoint Protection 策略可用于配置 Windows 设备的 Bitlocker 加密设置。</span><span class="sxs-lookup"><span data-stu-id="51389-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="51389-104">有关详细信息，请参阅 [Windows 10 (和更高版本) 设置，以使用 Intune 保护设备](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。</span><span class="sxs-lookup"><span data-stu-id="51389-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="51389-105">应注意，许多运行 Windows 10 的更新的设备都支持自动 Bitlocker 加密，这是在不应用 MDM 策略的情况下触发的。</span><span class="sxs-lookup"><span data-stu-id="51389-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="51389-106">如果配置了非默认设置，这可能会影响策略的应用。</span><span class="sxs-lookup"><span data-stu-id="51389-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="51389-107">有关更多详细信息，请参阅以下 FAQ。</span><span class="sxs-lookup"><span data-stu-id="51389-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="51389-108">有关对 bitlocker 问题进行故障排除的信息，请参阅 [Microsoft Intune 中的 bitlocker 策略疑难解答](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。</span><span class="sxs-lookup"><span data-stu-id="51389-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="51389-109">**常见问题解答**</span><span class="sxs-lookup"><span data-stu-id="51389-109">**FAQ**</span></span>

 <span data-ttu-id="51389-110">问：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？</span><span class="sxs-lookup"><span data-stu-id="51389-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="51389-111">A： Intune Endpoint Protection 策略中的设置是使用 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)实现的。</span><span class="sxs-lookup"><span data-stu-id="51389-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="51389-112">并不是所有版本或 Windows 版本都支持 Bitlocker CSP。</span><span class="sxs-lookup"><span data-stu-id="51389-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="51389-113">目前，支持以下 Windows 版本：企业版、教育版、移动版、移动企业版和专业版 (内部版本1809及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="51389-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="51389-114">问：如果已使用 OS 默认的加密方法和密码强度 (XTS-128) 加密了设备，则应用具有不同设置的策略将自动触发对具有新设置的驱动器的重新加密。</span><span class="sxs-lookup"><span data-stu-id="51389-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="51389-115">答：不可以。</span><span class="sxs-lookup"><span data-stu-id="51389-115">A: No.</span></span> <span data-ttu-id="51389-116">若要应用新密码设置，必须先解密驱动器。</span><span class="sxs-lookup"><span data-stu-id="51389-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="51389-117">**注意：** 对于使用 Autopilot 注册的设备，在对 Intune 策略进行评估之前不会触发在 OOBE 期间进行的自动加密，这将允许使用基于策略的设置来替代 OS 默认值。</span><span class="sxs-lookup"><span data-stu-id="51389-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="51389-118">问：如果某个设备因 Intune 策略的应用程序而被加密，则在删除该策略时是否会对其进行解密？</span><span class="sxs-lookup"><span data-stu-id="51389-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="51389-119">A：删除与加密相关的策略不会导致对配置的驱动器进行解密。</span><span class="sxs-lookup"><span data-stu-id="51389-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="51389-120">问：为什么 Intune 合规性策略显示我的设备未启用 Bitlocker，尽管它是吗？</span><span class="sxs-lookup"><span data-stu-id="51389-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="51389-121">A： Intune 合规性策略中的 "Bitlocker enabled" 设置使用 Windows 设备运行状况证明 (DHA) 客户端。</span><span class="sxs-lookup"><span data-stu-id="51389-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="51389-122">此客户端仅在引导时测量设备状态。</span><span class="sxs-lookup"><span data-stu-id="51389-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="51389-123">因此，如果 Bitlocker 加密完成后设备尚未重新启动，则 DHA 客户端服务不会将 Bitlocker 报告为活动状态。</span><span class="sxs-lookup"><span data-stu-id="51389-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 