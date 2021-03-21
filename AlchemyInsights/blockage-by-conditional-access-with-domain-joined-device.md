---
title: 由于使用已加入域的设备被条件访问阻止
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965459"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="19d4e-102">由于使用已加入域的设备被条件访问阻止</span><span class="sxs-lookup"><span data-stu-id="19d4e-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="19d4e-103">**强烈建议使用的工具**</span><span class="sxs-lookup"><span data-stu-id="19d4e-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="19d4e-104">[设备注册疑难解答工具](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 一可帮助解决最常见设备注册问题的工具。</span><span class="sxs-lookup"><span data-stu-id="19d4e-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="19d4e-105">[测试设备注册连接脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 此脚本有助于确保设备可以访问系统帐户下的设备注册终结点。</span><span class="sxs-lookup"><span data-stu-id="19d4e-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="19d4e-106">[Azure AD 设备清理脚本](https://github.com/mzmaili/AzureADDeviceCleanup) - 此脚本可用于查找和管理环境中过时的设备。</span><span class="sxs-lookup"><span data-stu-id="19d4e-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="19d4e-107">以下是为什么有条件访问可能会使已加入域的设备（混合 Azure AD）失败的一些常见原因。</span><span class="sxs-lookup"><span data-stu-id="19d4e-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="19d4e-108">**设备上没有 Azure AD PRT** - 需要确保设备具有 Azure AD 主刷新令牌 （PRT）。</span><span class="sxs-lookup"><span data-stu-id="19d4e-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="19d4e-109">有关 PRT 的详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="19d4e-110">若要验证是否具有 Azure AD PRT，可以在设备上运行 `dsregcmd/status` 命令，并验证 “AzureAdPrt” 是否等于 “YES”。</span><span class="sxs-lookup"><span data-stu-id="19d4e-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="19d4e-111">如果"AzureAdPrt"为"NO"，请检查以下内容：</span><span class="sxs-lookup"><span data-stu-id="19d4e-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="19d4e-112">**是否拥有含有 AD FS 的联合环境，并且访问用户的家庭网络**：在这种情况下，请确保从 Extranet 可以访问 "usernamemixed"终结点。</span><span class="sxs-lookup"><span data-stu-id="19d4e-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="19d4e-113">如果 AD FS 位于 VPN 后，请确保用户连接到 VPN，然后重新登录到设备。</span><span class="sxs-lookup"><span data-stu-id="19d4e-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="19d4e-114">有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="19d4e-115">**设备的 TPM 是否有故障，因此无法验证设备**：检查 "tpm.msc" 以查看 TPM 的状态是否为“就绪”。</span><span class="sxs-lookup"><span data-stu-id="19d4e-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="19d4e-116">如果不是，请运行 `dsregcmd/leave`，然后让设备重新加入 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="19d4e-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="19d4e-117">之后再重试。</span><span class="sxs-lookup"><span data-stu-id="19d4e-117">Then, try again.</span></span> <span data-ttu-id="19d4e-118">有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="19d4e-119">**你使用的是第三方标识提供程序，此提供程序不支持 WS-Trust 协议**。</span><span class="sxs-lookup"><span data-stu-id="19d4e-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="19d4e-120">如我们的文档所述，在这种情况下，混合使用 Azure AD 的混合设备无法正常工作。</span><span class="sxs-lookup"><span data-stu-id="19d4e-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="19d4e-121">请与标识提供者合作以获取支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="19d4e-122">**用户使用的是没有 Windows 10 帐户的 Chrome 浏览器** 或 **Office 扩展 Chrome 不会自动在加入 AAD 的设备或加入 AAD 的混合设备上自动使用 PRT**：这会导致任何基于设备的条件访问策略失败，并显示“未注册的设备”错误消息。</span><span class="sxs-lookup"><span data-stu-id="19d4e-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="19d4e-123">如果要正确使用 Chrome 浏览器，必须通过 SCCM 或 Intune 安装 “Windows 10 帐户”或“ 用户 Chrome 浏览器的 Office 扩展”。</span><span class="sxs-lookup"><span data-stu-id="19d4e-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="19d4e-124">有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="19d4e-125">如果无法远程推送扩展，请通知用户手动安装上述扩展之一，以访问基于设备的条件访问后面的应用程序。</span><span class="sxs-lookup"><span data-stu-id="19d4e-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="19d4e-126">有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="19d4e-127">**此设备已正确建立混合 Azure AD 联接，但是由于 Azure AD Connect 或 Azure 门户中的同步更改而无意中将其删除或禁用**：如果发生这种情况，即使 "AzureAdJoined" 和 "PRT" 状态在设备上显示为有效，此设备对象也不再被识别为完全连接的设备。</span><span class="sxs-lookup"><span data-stu-id="19d4e-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="19d4e-128">若要解决此问题，请在受影响的设备上运行 `dsregcmd/leave`，然后让它们重新加入 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="19d4e-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="19d4e-129">有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="19d4e-130">如果设备是 Windows 10 1809 更新版本，且具有VPN / Cloud 代理，并且看到 "AzureAdPrt" 状态的问题或任何具有SSO问题的应用程序（即使拥有PRT，也无法连接到邮箱），确保拥有此修补程序 [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2)或四月累积更新 [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)，以防止这些计算机上的 PRT 失败。</span><span class="sxs-lookup"><span data-stu-id="19d4e-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















