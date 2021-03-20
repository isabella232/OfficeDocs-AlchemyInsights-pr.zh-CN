---
title: Azure AD 联接设备的单一登录疑难解答
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897549"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="1c4e4-102">Azure AD 联接设备的单一登录疑难解答</span><span class="sxs-lookup"><span data-stu-id="1c4e4-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="1c4e4-103">如果你有本地 Active Directory (AD) 环境，并且你想要将加入 AD 域的计算机加入 Azure AD，则可以通过执行混合 Azure AD 加入来实现此目的。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="1c4e4-104">[How To： Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="1c4e4-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="1c4e4-105">有关详细信息，请参阅 Configure [Azure AD joined devices for on-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="1c4e4-106">**PRT (主要刷新) 问题**</span><span class="sxs-lookup"><span data-stu-id="1c4e4-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="1c4e4-107">主刷新令牌 (PRT) 是 Windows 10、Windows Server 2016 和更高版本、iOS 和 Android 设备上的 Azure AD 身份验证的关键项目。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="1c4e4-108">它是一个 JSON Web 令牌 (JWT) ，专门颁发给 Microsoft 第一方令牌代理，以在这些设备上使用的应用程序之间启用单一登录 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="1c4e4-109">有关如何在 Windows 10 设备上颁发、使用和保护 PRT 的详细信息，请参阅什么是[主刷新令牌？。](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="1c4e4-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="1c4e4-110">**WamDefaultSet：YES 和 AzureADPrt：YES**</span><span class="sxs-lookup"><span data-stu-id="1c4e4-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="1c4e4-111">这些字段指示用户登录设备时是否已成功通过 Azure AD 身份验证。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="1c4e4-112">如果值为 **NO，** 则可能是由于：</span><span class="sxs-lookup"><span data-stu-id="1c4e4-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="1c4e4-113">注册时与设备关联的 TPM 中的存储密钥 (在运行提升的设备时检查 KeySignTest) </span><span class="sxs-lookup"><span data-stu-id="1c4e4-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="1c4e4-114">备用登录 ID</span><span class="sxs-lookup"><span data-stu-id="1c4e4-114">Alternate Login ID</span></span>
- <span data-ttu-id="1c4e4-115">找不到 HTTP 代理</span><span class="sxs-lookup"><span data-stu-id="1c4e4-115">HTTP Proxy not found</span></span>

<span data-ttu-id="1c4e4-116">若要使用 dsregcmd 命令对设备进行故障排除，请参阅 [SSO 状态](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。</span><span class="sxs-lookup"><span data-stu-id="1c4e4-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
