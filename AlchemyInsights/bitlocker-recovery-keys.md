---
title: Bitlocker 恢复密钥
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820276"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="48518-102">访问 Bitlocker 恢复密钥</span><span class="sxs-lookup"><span data-stu-id="48518-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="48518-103">配置 Bitlocker 设置 Intune Endpoint Protection 策略时，可以定义 Bitlocker 恢复信息是否应该存储在 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="48518-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="48518-104">如果配置了该设置，则作为 Intune 设备边栏选项卡中的设备记录数据的一部分，存储的恢复数据应该对 Intune 管理员可见：</span><span class="sxs-lookup"><span data-stu-id="48518-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="48518-105">设备 - Azure AD 设备 ->"设备"或设备 -> 所有设备 ->"设备"->恢复密钥</span><span class="sxs-lookup"><span data-stu-id="48518-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="48518-106">或者，如果存在对设备本身的管理访问权限，则可以通过从提升的命令提示符 (以下命令来看到恢复密钥"密码) 密码"：</span><span class="sxs-lookup"><span data-stu-id="48518-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="48518-107">如果设备在 Intune 中注册之前已加密，恢复密钥可能与"Microsoft 帐户" (MSA) 用于在 OOBE 过程中登录到设备。</span><span class="sxs-lookup"><span data-stu-id="48518-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="48518-108">如果是这种情况，则通过该 MSA 访问和登录应显示存储了恢复  https://onedrive.live.com/recoverykey 密钥的设备。</span><span class="sxs-lookup"><span data-stu-id="48518-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="48518-109">如果设备是通过基于域的组策略进行配置而加密的，则恢复信息可能存储在本地 Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="48518-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="48518-110">如果你已配置终结点保护策略以将恢复密钥存储在 Azure Active Directory 中，但特定设备的密钥尚未上载，则可以通过从 MEM 控制台旋转该设备的恢复密钥来触发上传。</span><span class="sxs-lookup"><span data-stu-id="48518-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="48518-111">有关详细信息，请参阅 [旋转 BitLocker 恢复密钥](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)。</span><span class="sxs-lookup"><span data-stu-id="48518-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

