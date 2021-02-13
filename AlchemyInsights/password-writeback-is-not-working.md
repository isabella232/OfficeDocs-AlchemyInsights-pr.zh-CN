---
title: 密码写回无法工作
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232663"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="219d2-102">密码写回无法工作</span><span class="sxs-lookup"><span data-stu-id="219d2-102">Password Writeback is not working</span></span>

<span data-ttu-id="219d2-103">**我在配置密码写回时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="219d2-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="219d2-104">密码写回是一项高级功能。</span><span class="sxs-lookup"><span data-stu-id="219d2-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="219d2-105">确保您了解许可要求：</span><span class="sxs-lookup"><span data-stu-id="219d2-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="219d2-106">必须在组织中分配至少一个许可证</span><span class="sxs-lookup"><span data-stu-id="219d2-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="219d2-107">**仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="219d2-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="219d2-108">**云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) </span><span class="sxs-lookup"><span data-stu-id="219d2-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="219d2-109">若要了解有关许可要求的信息，请参阅[Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)自助服务密码重置的许可要求</span><span class="sxs-lookup"><span data-stu-id="219d2-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="219d2-110">您至少有一个管理员帐户和一个具有相应许可证之一的测试用户帐户。</span><span class="sxs-lookup"><span data-stu-id="219d2-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="219d2-111">必须将 Azure AD Connect 连接到主域控制器仿真器，密码写回才能工作。</span><span class="sxs-lookup"><span data-stu-id="219d2-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="219d2-112">可以通过右键单击 Active Directory 同步连接器的属性，然后选择配置目录分区，将 Azure AD Connect 配置为使用主 **域控制器**。</span><span class="sxs-lookup"><span data-stu-id="219d2-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="219d2-113">从该位置查找 **域控制器连接设置** 部分，并选中标题仅使用首选域控制器 **的框**。</span><span class="sxs-lookup"><span data-stu-id="219d2-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="219d2-114">如果首选 DC 不是 PDC 仿真器，Azure AD Connect 仍将联系 PDC 进行密码写回。</span><span class="sxs-lookup"><span data-stu-id="219d2-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="219d2-115">已在租户中配置和启用密码重置。</span><span class="sxs-lookup"><span data-stu-id="219d2-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="219d2-116">有关详细信息，请参阅"[允许用户重置其 Azure AD 密码"。](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="219d2-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="219d2-117">确保用于启用密码写回的管理员帐户是在 Azure AD (本地 AD 帐户创建的云管理员) </span><span class="sxs-lookup"><span data-stu-id="219d2-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="219d2-118">你拥有运行 Windows Server 2008 R2、Windows Server 2012 或 Windows Server 2012 R2 的单个或多林 AD 本地部署，并安装了最新的 Service Pack</span><span class="sxs-lookup"><span data-stu-id="219d2-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="219d2-119">已安装 Azure AD Connect 工具，并且已准备 AD 环境以同步到云。</span><span class="sxs-lookup"><span data-stu-id="219d2-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="219d2-120">在测试密码写回之前，请确保首先从 Azure AD Connect 中的 AD 和 Azure AD 完成完全导入和完全同步。</span><span class="sxs-lookup"><span data-stu-id="219d2-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="219d2-121">若要了解更多信息，请参阅如何在 Azure [AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)中执行完全同步和完全导入</span><span class="sxs-lookup"><span data-stu-id="219d2-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="219d2-122">**密码写回连接出现问题**</span><span class="sxs-lookup"><span data-stu-id="219d2-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="219d2-123">下载并启用 [最新版本的 Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="219d2-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="219d2-124">防火墙配置：Azure AD Connect (1.1.443 及) 将需要出 **站 HTTPS** 访问权限：</span><span class="sxs-lookup"><span data-stu-id="219d2-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="219d2-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="219d2-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="219d2-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="219d2-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="219d2-127">允许空闲连接至少保留 2-3 分钟</span><span class="sxs-lookup"><span data-stu-id="219d2-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="219d2-128">**我仍遇到密码写回问题**</span><span class="sxs-lookup"><span data-stu-id="219d2-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="219d2-129">如果仍有问题，请尝试在 Azure AD Connect 工具中禁用和重新启用密码写回服务</span><span class="sxs-lookup"><span data-stu-id="219d2-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="219d2-130">若要了解更多信息，请参阅如何 [禁用和重新启用密码写回](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="219d2-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
