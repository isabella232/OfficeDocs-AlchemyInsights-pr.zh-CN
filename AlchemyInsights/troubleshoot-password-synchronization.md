---
title: 密码同步疑难解答
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533797"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="32f83-102">密码同步疑难解答</span><span class="sxs-lookup"><span data-stu-id="32f83-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="32f83-103">若要解决没有与 Azure AD Connect 版本1.1.614.0 或更高版本同步的密码的问题, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="32f83-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="32f83-104">使用 "以**管理员身份运行**" 选项在 Azure AD Connect 服务器上打开新的 Windows PowerShell 会话。</span><span class="sxs-lookup"><span data-stu-id="32f83-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="32f83-105">运行**ExecutionPolicy RemoteSigned**或 ExecutionPolicy 不**受限制的设置**。</span><span class="sxs-lookup"><span data-stu-id="32f83-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="32f83-106">启动 Azure AD Connect 向导。</span><span class="sxs-lookup"><span data-stu-id="32f83-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="32f83-107">导航到 "**其他任务**" 页, 选择 "**疑难解答**", 然后单击 "**下一步**"。</span><span class="sxs-lookup"><span data-stu-id="32f83-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="32f83-108">在 "疑难解答" 页上, 单击 "**启动" 以启动 PowerShell 中的 "疑难解答"** 菜单。</span><span class="sxs-lookup"><span data-stu-id="32f83-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="32f83-109">在主菜单中, 选择 "**密码同步疑难解答**"。</span><span class="sxs-lookup"><span data-stu-id="32f83-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="32f83-110">在子菜单中, 选择 "**密码同步" 根本不起作用**。</span><span class="sxs-lookup"><span data-stu-id="32f83-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="32f83-111">**了解故障排除任务的结果**</span><span class="sxs-lookup"><span data-stu-id="32f83-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="32f83-112">故障排除任务将执行以下检查:</span><span class="sxs-lookup"><span data-stu-id="32f83-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="32f83-113">验证是否已为 Azure AD 租户启用密码同步功能。</span><span class="sxs-lookup"><span data-stu-id="32f83-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="32f83-114">验证 Azure AD Connect 服务器是否未处于暂存模式。</span><span class="sxs-lookup"><span data-stu-id="32f83-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="32f83-115">对于每个现有的本地 Active Directory 连接器 (对应于现有的 Active Directory 林):</span><span class="sxs-lookup"><span data-stu-id="32f83-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="32f83-116">验证是否已启用密码同步功能。</span><span class="sxs-lookup"><span data-stu-id="32f83-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="32f83-117">在 Windows 应用程序事件日志中搜索密码同步检测信号事件。</span><span class="sxs-lookup"><span data-stu-id="32f83-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="32f83-118">对于内部部署 Active Directory 连接器下的每个 Active Directory 域:</span><span class="sxs-lookup"><span data-stu-id="32f83-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="32f83-119">验证是否可以从 Azure AD Connect 服务器访问域。</span><span class="sxs-lookup"><span data-stu-id="32f83-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="32f83-120">验证本地 Active Directory 连接器使用的 Active Directory 域服务 (AD DS) 帐户是否具有密码同步所需的正确用户名、密码和权限。</span><span class="sxs-lookup"><span data-stu-id="32f83-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="32f83-121">有关疑难解答密码同步的更多帮助, 请参阅[密码同步与 AZURE AD Connect Sync 疑难解答](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="32f83-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  