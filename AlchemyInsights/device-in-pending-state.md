---
title: 设备挂起状态
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652124"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="09b7a-102">设备挂起状态</span><span class="sxs-lookup"><span data-stu-id="09b7a-102">Device in pending state</span></span>

<span data-ttu-id="09b7a-103">**先决条件：**</span><span class="sxs-lookup"><span data-stu-id="09b7a-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="09b7a-104">如果是首次设置设备注册，请确保已查看 [Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 中的设备管理简介，该简介将指导你如何获取受 Azure AD 控制的设备。</span><span class="sxs-lookup"><span data-stu-id="09b7a-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="09b7a-105">如果你直接将设备注册到 Azure AD 并注册到 Intune 中，你将需要确保你已配置[Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)并首先获得许可[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="09b7a-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="09b7a-106">确保你有权在 Azure AD 和本地 AD 中执行操作。</span><span class="sxs-lookup"><span data-stu-id="09b7a-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="09b7a-107">只有 Azure AD 中的全局管理员可以管理设备注册的设置。</span><span class="sxs-lookup"><span data-stu-id="09b7a-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="09b7a-108">此外，如果要在本地 Active Directory 中设置自动注册，则需要是 Active Directory 和 AD FS (管理员（如果适用) ）。</span><span class="sxs-lookup"><span data-stu-id="09b7a-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="09b7a-109">混合 Azure AD 加入注册过程要求设备位于企业网络中。</span><span class="sxs-lookup"><span data-stu-id="09b7a-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="09b7a-110">它还适用于 VPN，但需要注意一些问题。</span><span class="sxs-lookup"><span data-stu-id="09b7a-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="09b7a-111">我们听到客户需要协助解决远程工作环境下的混合 Azure AD 加入注册过程。</span><span class="sxs-lookup"><span data-stu-id="09b7a-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="09b7a-112">**云身份验证环境 (Azure AD 密码哈希同步或传递身份验证)**</span><span class="sxs-lookup"><span data-stu-id="09b7a-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="09b7a-113">此注册流也称为"同步加入"。</span><span class="sxs-lookup"><span data-stu-id="09b7a-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="09b7a-114">以下是注册过程中所发生事情的细目：</span><span class="sxs-lookup"><span data-stu-id="09b7a-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="09b7a-115">Windows 10 在用户登录 (SCP) 发现服务连接点。</span><span class="sxs-lookup"><span data-stu-id="09b7a-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="09b7a-116">设备首先尝试从注册表中的客户端 SCP 检索租户信息 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。</span><span class="sxs-lookup"><span data-stu-id="09b7a-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="09b7a-117">有关详细信息，请参阅 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。</span><span class="sxs-lookup"><span data-stu-id="09b7a-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="09b7a-118">如果失败，设备会与本地 Active Directory 通信，以从 SCP 获取租户信息。</span><span class="sxs-lookup"><span data-stu-id="09b7a-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="09b7a-119">若要验证 SCP，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。</span><span class="sxs-lookup"><span data-stu-id="09b7a-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="09b7a-120">我们建议在 Active Directory 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。</span><span class="sxs-lookup"><span data-stu-id="09b7a-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="09b7a-121">Windows 10 尝试在系统上下文中与 Azure AD 进行通信，以针对 Azure AD 自行进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="09b7a-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="09b7a-122">可以使用测试设备注册连接脚本验证设备能否访问系统帐户下的 Microsoft [资源](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)。</span><span class="sxs-lookup"><span data-stu-id="09b7a-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="09b7a-123">Windows 10 生成自签名证书，并存储在本地 Active Directory 中的计算机对象下。</span><span class="sxs-lookup"><span data-stu-id="09b7a-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="09b7a-124">这需要域控制器的视线。</span><span class="sxs-lookup"><span data-stu-id="09b7a-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="09b7a-125">具有证书的设备对象通过 Azure AD Connect 同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="09b7a-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="09b7a-126">默认情况下，同步周期是每 30 分钟一次，但它取决于 Azure AD Connect 的配置。</span><span class="sxs-lookup"><span data-stu-id="09b7a-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="09b7a-127">有关详细信息，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。</span><span class="sxs-lookup"><span data-stu-id="09b7a-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="09b7a-128">在此阶段，你应该能够在 Azure 门户的设备边栏选项卡下看到主题设备处于"挂起"状态。</span><span class="sxs-lookup"><span data-stu-id="09b7a-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="09b7a-129">下次用户登录到 Windows 10 时，将完成注册。</span><span class="sxs-lookup"><span data-stu-id="09b7a-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="09b7a-130">如果你使用 VPN 并且注销/登录终止了域连接，你可以手动触发注册。</span><span class="sxs-lookup"><span data-stu-id="09b7a-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="09b7a-131">为此，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="09b7a-131">To do that:</span></span>
    >
    > <span data-ttu-id="09b7a-132">在本地 `dsregcmd /join` 管理员提示或通过 PSExec 远程向电脑发出。</span><span class="sxs-lookup"><span data-stu-id="09b7a-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="09b7a-133">例如：`PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="09b7a-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="09b7a-134">有关 Azure Active Directory 设备注册的常见问题，请参阅 [设备常见问题](https://docs.microsoft.com/azure/active-directory/devices/faq)解答。</span><span class="sxs-lookup"><span data-stu-id="09b7a-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
