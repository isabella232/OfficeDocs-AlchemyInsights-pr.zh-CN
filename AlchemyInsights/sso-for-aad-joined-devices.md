---
title: Single-Sign加入 Azure Active Directory 的设备打开
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403780"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="7b33b-102">加入 Azure Active Directory 的设备的单一登录</span><span class="sxs-lookup"><span data-stu-id="7b33b-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="7b33b-103">如果你有本地 Active Directory (AD) 环境，并且你想要将加入 AD 域的计算机加入 Azure AD，则可以通过执行混合 Azure AD 加入来实现此目的。</span><span class="sxs-lookup"><span data-stu-id="7b33b-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="7b33b-104">[How To： Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="7b33b-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="7b33b-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="7b33b-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="7b33b-106">**PRT (主要刷新) 问题** 主刷新令牌 (PRT) 是 Windows 10、Windows Server 2016 和更高版本、iOS 和 Android 设备上的 Azure AD 身份验证的关键项目。</span><span class="sxs-lookup"><span data-stu-id="7b33b-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="7b33b-107">它是一个 JSON Web 令牌 (JWT) ，专门颁发给 Microsoft 第一方令牌代理，以在这些设备上使用的应用程序之间启用单一登录 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="7b33b-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="7b33b-108">[在什么是主刷新令牌？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)中，我们将详细介绍如何在 Windows 10 设备上颁发、使用和保护 PRT。</span><span class="sxs-lookup"><span data-stu-id="7b33b-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="7b33b-109">**WamDefaultSet：YES 和 AzureADPrt：YES** 这些字段指示用户登录设备时是否已成功通过 Azure AD 身份验证。</span><span class="sxs-lookup"><span data-stu-id="7b33b-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="7b33b-110">如果值为 **NO，** 则可能是由于：</span><span class="sxs-lookup"><span data-stu-id="7b33b-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="7b33b-111">注册时与设备关联的 TPM 中的存储密钥 (在运行提升的设备时检查 KeySignTest) 。</span><span class="sxs-lookup"><span data-stu-id="7b33b-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="7b33b-112">备用登录 ID</span><span class="sxs-lookup"><span data-stu-id="7b33b-112">Alternate Login ID</span></span>
- <span data-ttu-id="7b33b-113">找不到 HTTP 代理</span><span class="sxs-lookup"><span data-stu-id="7b33b-113">HTTP Proxy not found</span></span>

<span data-ttu-id="7b33b-114">使用 dsregcmd 命令对设备进行故障排除 - [SSO 状态](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="7b33b-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
