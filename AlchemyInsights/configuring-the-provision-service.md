---
title: 配置预配服务
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480744"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="b6cd3-102">配置预配服务</span><span class="sxs-lookup"><span data-stu-id="b6cd3-102">Configuring the Provision service</span></span>

<span data-ttu-id="b6cd3-103">若要使自动用户预配正常工作，Azure AD 需要允许其连接到 Workday Web 服务 API 的有效凭据。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="b6cd3-104">此外，Workday 到 AD 用户预配应用的"测试连接"按钮还会验证它能否连接到与 AD 域关联的 Azure AD Connect 预配代理。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="b6cd3-105">如果 Azure 门户在保存凭据时返回错误，请按照下面的建议步骤操作：</span><span class="sxs-lookup"><span data-stu-id="b6cd3-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="b6cd3-106">确认你已配置 Workday 集成系统用户帐户，如教程部分所述在 [Workday 中配置集成系统用户](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="b6cd3-107">使用服务管理控制台确认 Azure AD Connect 预配代理服务已在本地 Windows 服务器上启动并运行。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="b6cd3-108">还可以单击"查看本地代理"按钮，在 Azure 门户中检查代理的状态。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="b6cd3-109">确保使用"工作日用户名"字段的格式输入username@workday-tenant-name。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="b6cd3-110">如果缺少 workday-tenant-name，则 Workday 身份验证将失败。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="b6cd3-111">如果要配置与 Workday 实现租户的集成，请注意 Workday 租户的计划停机时间。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="b6cd3-112">工作日已安排其实施租户在周末的停机时间 (通常从星期五晚上到星期六上午) 并且此停机时间窗口中的连接故障是一个已知问题，一旦实现租户重新联机，就会自动解决该问题。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="b6cd3-113">在极少数情况下，如果集成系统用户的密码因租户刷新而更改，或者帐户已锁定或已过期，则也可能看到此错误。</span><span class="sxs-lookup"><span data-stu-id="b6cd3-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="b6cd3-114">Please check the status of the Integration System user with your Workday administrator.</span><span class="sxs-lookup"><span data-stu-id="b6cd3-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="b6cd3-115">有关为自动预配配置工作日的更多详细信息，请参阅教程：为自动用户预配配置[Workday。](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="b6cd3-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
