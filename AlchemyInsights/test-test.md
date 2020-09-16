---
title: SharePoint Online 术语库中缺少术语
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750441"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="311c1-102">使用 Intune 启用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="311c1-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="311c1-103">Intune Endpoint Protection 策略可用于为 Windows 设备配置 Boitlocker 加密设置，如中所述： Windows10 (and 更高版本使用 Intune 保护设备) 设置</span><span class="sxs-lookup"><span data-stu-id="311c1-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="311c1-104">应注意，许多运行 Windows 10 的更新的设备支持自动 bitlocker 加密，而无需应用 MDM 策略触发。</span><span class="sxs-lookup"><span data-stu-id="311c1-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="311c1-105">如果配置了非默认设置，这可能会影响策略的应用。</span><span class="sxs-lookup"><span data-stu-id="311c1-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="311c1-106">请参阅 FAQ 以了解更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="311c1-106">See FAQ for more detail.</span></span>


<span data-ttu-id="311c1-107">FAQ   Q：哪些版本的 Windows 支持使用 Endpoint Protection 策略进行设备加密？</span><span class="sxs-lookup"><span data-stu-id="311c1-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="311c1-108"> A： Intune Endpoint Protection 策略中的设置是使用 Bitlocker CSP 实现的。</span><span class="sxs-lookup"><span data-stu-id="311c1-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="311c1-109">并非所有版本的 Windows 都支持 Bitlocker CSP。 
     </span><span class="sxs-lookup"><span data-stu-id="311c1-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="311c1-110">在这段时间，Windows 版本为：企业版;支持从内部版本1809开始) 教育、移动、移动企业和专业 (。</span><span class="sxs-lookup"><span data-stu-id="311c1-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="311c1-111">问：如果已使用 OS 默认的加密方法和密码强度的 XTS 默认设置为设备加密了一个设备，则 (-128) 将应用具有不同设置的策略自动触发对该驱动器的重新加密使用新设置？</span><span class="sxs-lookup"><span data-stu-id="311c1-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="311c1-112">答：不可以。</span><span class="sxs-lookup"><span data-stu-id="311c1-112">A: No.</span></span> <span data-ttu-id="311c1-113">若要应用新密码设置，必须先解密驱动器。</span><span class="sxs-lookup"><span data-stu-id="311c1-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="311c1-114">注意：对于使用 Autopilot 注册的设备，在对 Intune 策略进行评估时，将不会触发在 OOBE 期间进行的自动加密，这将允许使用基于策略的设置替代 OS 默认值</span><span class="sxs-lookup"><span data-stu-id="311c1-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="311c1-115">问：如果某个设备因 Intune 策略的应用程序而被加密，则在删除该策略时将对其进行解密？</span><span class="sxs-lookup"><span data-stu-id="311c1-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="311c1-116">A：删除与加密相关的策略不会导致对配置的驱动器进行解密。</span><span class="sxs-lookup"><span data-stu-id="311c1-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="311c1-117">问：为什么 intune 合规性策略显示我的设备不具有 "Bitlocker 已启用"，但它是什么？</span><span class="sxs-lookup"><span data-stu-id="311c1-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="311c1-118">A： intune 合规性策略中的 "Bitlocker enabled" 设置利用 Windows 设备运行状况证明 (DHA) 客户端。</span><span class="sxs-lookup"><span data-stu-id="311c1-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="311c1-119">此客户端仅在引导时测量设备状态。</span><span class="sxs-lookup"><span data-stu-id="311c1-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="311c1-120">因此，如果 bitlocker 加密完成后设备尚未重新启动，则 DHA 客户端服务不会将 bitlocker 报告为活动状态。</span><span class="sxs-lookup"><span data-stu-id="311c1-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>