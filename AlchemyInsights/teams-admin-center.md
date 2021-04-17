---
title: Teams 管理中心
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826369"
---
# <a name="teams-admin-center"></a><span data-ttu-id="0dee0-102">Teams 管理中心</span><span class="sxs-lookup"><span data-stu-id="0dee0-102">Teams Admin Center</span></span>

<span data-ttu-id="0dee0-103">了解如何通过 [Teams 管理中心](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)管理 Teams。</span><span class="sxs-lookup"><span data-stu-id="0dee0-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="0dee0-104">如果无法访问 Teams 管理中心，请检查以下项：</span><span class="sxs-lookup"><span data-stu-id="0dee0-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="0dee0-105">验证是否已在任何外围设备（防火墙等）上或在本地计算机的防火墙规则中允许相应的 [Office 365 IP 地址和 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)。</span><span class="sxs-lookup"><span data-stu-id="0dee0-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="0dee0-106">验证用于访问 Teams 管理门户的登录名与 [Microsoft 365 管理门户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中列出的用户名是否匹配。</span><span class="sxs-lookup"><span data-stu-id="0dee0-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="0dee0-107">如果用户未出现在埃 Teams 管理中心，请检查以下项：</span><span class="sxs-lookup"><span data-stu-id="0dee0-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="0dee0-108">是否在最近 24 小时内创建了用户或分配了许可证？</span><span class="sxs-lookup"><span data-stu-id="0dee0-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="0dee0-109">请确保在打开支持票证前等待至少 24 小时。</span><span class="sxs-lookup"><span data-stu-id="0dee0-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="0dee0-110">验证是否分配了适当的许可证？</span><span class="sxs-lookup"><span data-stu-id="0dee0-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="0dee0-111">如果你有一个本地 Active Directory，请确认 [本地 Active Directory 中 ProxyAddresses 字段中的 msRTCSIP-PrimaryUserAddress 或 SIP 地址的值是唯一的，并且格式匹配](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip：来自 [Microsoft 365 管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中用户的 **用户名**。</span><span class="sxs-lookup"><span data-stu-id="0dee0-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="0dee0-112">如果你打算保留 Skype for Business Server 部署，并且让用户驻留在本地和联机：请按照 Skype for Business Server 控制面板中的“**使用 Teams 和 Skype for Business Online 设置混合**” ，并联机移动用户。</span><span class="sxs-lookup"><span data-stu-id="0dee0-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
