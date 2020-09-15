---
title: Intune Wi-Fi 配置文件
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696251"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="31724-102">Intune Wi-Fi 配置文件</span><span class="sxs-lookup"><span data-stu-id="31724-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="31724-103">MDM 客户端的 Wi-Fi 连接的成功实现依赖于可反映公司 Wi-Fi 基础结构要求的正确部署的配置文件。</span><span class="sxs-lookup"><span data-stu-id="31724-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="31724-104">若要查看正在调查的客户端平台的相应设置，请参阅：</span><span class="sxs-lookup"><span data-stu-id="31724-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="31724-105">在 Microsoft Intune 中为运行 Android 的设备添加 Wi-Fi 设置</span><span class="sxs-lookup"><span data-stu-id="31724-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="31724-106">在 Microsoft Intune 中为 Android 企业版专用且完全托管的设备添加 Wi-Fi 设置</span><span class="sxs-lookup"><span data-stu-id="31724-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="31724-107">在 Microsoft Intune 中为 iOS 和 iPadOS 设备添加 Wi-Fi 设置</span><span class="sxs-lookup"><span data-stu-id="31724-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="31724-108">在 Intune 中为 Windows 10 和更高版本的设备添加 Wi-Fi 设置</span><span class="sxs-lookup"><span data-stu-id="31724-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="31724-109">在 Intune 中为 Windows 设备导入 Wi-Fi 设置</span><span class="sxs-lookup"><span data-stu-id="31724-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="31724-110">**常见问题**</span><span class="sxs-lookup"><span data-stu-id="31724-110">**Common Issues**</span></span>

<span data-ttu-id="31724-111">**我正在部署的 Wi-Fi 配置文件依赖于该 Wi-Fi 配置文件中指定的已部署证书。但是，配置的配置文件显示错误状态。**</span><span class="sxs-lookup"><span data-stu-id="31724-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="31724-112">请检查你的设备是否收到了证书。</span><span class="sxs-lookup"><span data-stu-id="31724-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="31724-113">在 Intune 中，转到“**所有设备**”，然后选择选择相应设备 >“**设备配置**”。</span><span class="sxs-lookup"><span data-stu-id="31724-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="31724-114">检查是否列出了所有预期的配置文件，并且状态为成功。</span><span class="sxs-lookup"><span data-stu-id="31724-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="31724-115">对于 Android 配置文件，如果证书链中有中间证书，请确保将其部署到 Android 设备。</span><span class="sxs-lookup"><span data-stu-id="31724-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="31724-116">若要检查证书状态，请转到“**设备配置**” > “**配置文件**” > “**Android 中间 CA**” > “**属性**” > “**受信任的证书**”。</span><span class="sxs-lookup"><span data-stu-id="31724-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="31724-117">如果仍然出现错误，请查看过程和疑难解答部分。</span><span class="sxs-lookup"><span data-stu-id="31724-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="31724-118">有关详细信息，请参阅[有关使用 Microsoft Intune 解决 SCEP 证书配置文件问题的概述](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="31724-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="31724-119">**我已将 Wi-Fi 配置文件部署到设备。Intune 显示该操作已成功，但设备却未连接到 Wi-Fi。**</span><span class="sxs-lookup"><span data-stu-id="31724-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="31724-120">成功状态表示 Intune 已按照配置成功部署了配置文件。</span><span class="sxs-lookup"><span data-stu-id="31724-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="31724-121">但是，这些配置可能不符合您的网络和/或身份验证要求。</span><span class="sxs-lookup"><span data-stu-id="31724-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="31724-122">有关尝试的连接的更多详细信息，请查看基础结构和身份验证服务中的日志（在 Wi-Fi 接入点控制器和 NPS/Radius 服务器上）。</span><span class="sxs-lookup"><span data-stu-id="31724-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="31724-123">你可能需要与网络基础结构团队或第三方 Wi-Fi 供应商合作，以收集和查看日志。</span><span class="sxs-lookup"><span data-stu-id="31724-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>