---
title: 解决密码同步
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459428"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="de8ab-102">解决密码同步</span><span class="sxs-lookup"><span data-stu-id="de8ab-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="de8ab-103">若要解决其中没有密码都是同步与 Azure AD 连接版本 1.1.614.0 或更高版本的问题：</span><span class="sxs-lookup"><span data-stu-id="de8ab-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="de8ab-104">使用**以管理员身份运行**选项打开新 Azure AD 连接服务器上的 Windows PowerShell 会话。</span><span class="sxs-lookup"><span data-stu-id="de8ab-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="de8ab-105">运行**Set-executionpolicy RemoteSigned**或**不受限制的 Set-executionpolicy**。</span><span class="sxs-lookup"><span data-stu-id="de8ab-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="de8ab-106">启动 Azure AD 连接向导。</span><span class="sxs-lookup"><span data-stu-id="de8ab-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="de8ab-107">导航到 \* \* 其他任务 \* \* 页上，选择 \* \* Troubleshoot \* \*，，单击**下一步**。</span><span class="sxs-lookup"><span data-stu-id="de8ab-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="de8ab-108">在疑难解答页上，单击在 PowerShell 中的**启动启动疑难解答**菜单。</span><span class="sxs-lookup"><span data-stu-id="de8ab-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="de8ab-109">在主菜单中，选择**解决密码同步**。</span><span class="sxs-lookup"><span data-stu-id="de8ab-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="de8ab-110">在 sub 菜单中，选择**根本不起作用密码同步**。</span><span class="sxs-lookup"><span data-stu-id="de8ab-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="de8ab-111">**了解故障排除任务的结果**</span><span class="sxs-lookup"><span data-stu-id="de8ab-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="de8ab-112">故障排除任务可以执行以下检查：</span><span class="sxs-lookup"><span data-stu-id="de8ab-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="de8ab-113">验证已为您的 Azure AD 租户启用密码同步功能。</span><span class="sxs-lookup"><span data-stu-id="de8ab-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="de8ab-114">验证 Azure AD 连接服务器不是在调试模式。</span><span class="sxs-lookup"><span data-stu-id="de8ab-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="de8ab-115">对于每个现有内部部署 Active Directory 连接器 （其对应的现有的 Active Directory 林）：</span><span class="sxs-lookup"><span data-stu-id="de8ab-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="de8ab-116">验证已启用的密码同步功能。</span><span class="sxs-lookup"><span data-stu-id="de8ab-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="de8ab-117">搜索的 Windows 应用程序事件日志中的密码同步检测信号事件。</span><span class="sxs-lookup"><span data-stu-id="de8ab-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="de8ab-118">在内部部署 Active Directory 连接器下的每个 Active Directory 域：</span><span class="sxs-lookup"><span data-stu-id="de8ab-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="de8ab-119">验证域从 Azure AD 连接服务器上可以访问。</span><span class="sxs-lookup"><span data-stu-id="de8ab-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="de8ab-120">验证内部部署 Active Directory 连接器使用的 Active Directory 域服务 (AD DS) 帐户具有正确的用户名、 密码和所需的密码同步权限。</span><span class="sxs-lookup"><span data-stu-id="de8ab-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="de8ab-121">疑难解答密码同步的更多帮助，请参阅[Troubleshoot 与 Azure AD 连接同步的密码同步](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="de8ab-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

