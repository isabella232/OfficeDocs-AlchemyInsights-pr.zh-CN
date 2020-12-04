---
title: 解决 PRT 问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571820"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="efccf-102">解决 PRT 问题</span><span class="sxs-lookup"><span data-stu-id="efccf-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="efccf-103">若要使任何设备完成身份验证，必须完全注册并处于正常状态，并且能够 (PRT) 中获取主刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="efccf-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="efccf-104">混合 Azure AD 加入注册过程需要设备位于企业网络上。</span><span class="sxs-lookup"><span data-stu-id="efccf-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="efccf-105">它还通过 VPN 工作，但有一些注意事项。</span><span class="sxs-lookup"><span data-stu-id="efccf-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="efccf-106">我们已听取客户需要在远程工作环境中对混合 Azure AD 加入注册过程进行故障排除的帮助。</span><span class="sxs-lookup"><span data-stu-id="efccf-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="efccf-107">下面是在注册过程中对 "盖子" 下发生的事情的细目。</span><span class="sxs-lookup"><span data-stu-id="efccf-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="efccf-108">**使用 Azure AD 密码哈希同步或传递身份验证 (云身份验证环境)**</span><span class="sxs-lookup"><span data-stu-id="efccf-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="efccf-109">此注册流程也称为 "同步加入"。</span><span class="sxs-lookup"><span data-stu-id="efccf-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="efccf-110">Windows 10 在用户登录设备时发现 SCP 记录。</span><span class="sxs-lookup"><span data-stu-id="efccf-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="efccf-111">设备首先尝试从注册表 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] 中的客户端 SCP 检索租户信息。</span><span class="sxs-lookup"><span data-stu-id="efccf-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="efccf-112">有关详细信息，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。</span><span class="sxs-lookup"><span data-stu-id="efccf-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="efccf-113">如果失败，则设备与本地 Active Directory (AD) 通信，以从服务连接点 (SCP) 获取租户信息。</span><span class="sxs-lookup"><span data-stu-id="efccf-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="efccf-114">若要验证 SCP，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。</span><span class="sxs-lookup"><span data-stu-id="efccf-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="efccf-115">我们建议在 AD 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。</span><span class="sxs-lookup"><span data-stu-id="efccf-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="efccf-116">Windows 10 尝试在系统上下文中与 Azure AD 进行通信，以针对 Azure AD 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="efccf-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="efccf-117">您可以使用测试设备注册连接脚本来验证设备是否可以访问系统帐户下的 Microsoft 资源。</span><span class="sxs-lookup"><span data-stu-id="efccf-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="efccf-118">Windows 10 生成自签名证书，并将其存储在本地 AD 中的计算机对象下。</span><span class="sxs-lookup"><span data-stu-id="efccf-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="efccf-119">这需要向域控制器进行实时滚动。</span><span class="sxs-lookup"><span data-stu-id="efccf-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="efccf-120">具有证书的设备对象通过 Azure AD Connect 同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="efccf-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="efccf-121">默认情况下，同步周期每30分钟一次，但具体取决于 Azure AD Connect 的配置。</span><span class="sxs-lookup"><span data-stu-id="efccf-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="efccf-122">有关详细信息，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。</span><span class="sxs-lookup"><span data-stu-id="efccf-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="efccf-123">在此阶段，您应能够在 Azure 门户的设备刀片下的 "挂起" 状态中查看主题设备。</span><span class="sxs-lookup"><span data-stu-id="efccf-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="efccf-124">在下一个用户登录到 Windows 10 时，将完成注册。</span><span class="sxs-lookup"><span data-stu-id="efccf-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="efccf-125">如果你在 VPN 上且注销登录过程终止了域连接，则可以手动触发注册：</span><span class="sxs-lookup"><span data-stu-id="efccf-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="efccf-126">在管理员提示符处或远程通过 PSExec 将 dsregcmd/join 从本地发出到你的电脑。</span><span class="sxs-lookup"><span data-stu-id="efccf-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="efccf-127">例如，PsExec-s \\ win10client01 cmd，dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="efccf-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="efccf-128">有关混合加入问题的更多详细信息，请参阅 [设备问题故障排除](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)。</span><span class="sxs-lookup"><span data-stu-id="efccf-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
