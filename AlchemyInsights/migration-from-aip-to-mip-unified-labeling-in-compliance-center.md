---
title: 在合规中心从 AIP 迁移到 MIP/统一标签
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674316"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="8ab77-102">在合规中心从 AIP 迁移到 MIP/统一标签</span><span class="sxs-lookup"><span data-stu-id="8ab77-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="8ab77-103">若要在安全与合规中心从 AIP 标签迁移到统一标签，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="8ab77-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="8ab77-104">**从 Azure 门户激活保护**</span><span class="sxs-lookup"><span data-stu-id="8ab77-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="8ab77-105">如果尚未执行此操作，请打开一个新的浏览器窗口，然后[登录 Azure 门户](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="8ab77-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="8ab77-106">导航到“**Azure 信息保护**”边栏选项卡。</span><span class="sxs-lookup"><span data-stu-id="8ab77-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="8ab77-107">例如，在中心菜单上，单击“**所有服务**”并开始在“筛选器”框中键入**信息**。</span><span class="sxs-lookup"><span data-stu-id="8ab77-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="8ab77-108">选择“**Azure 信息保护**”。</span><span class="sxs-lookup"><span data-stu-id="8ab77-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="8ab77-109">如果之前未访问过“Azure 信息保护”边栏选项卡，请参阅一次性[其他步骤](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)，将此边栏选项卡添加到门户。</span><span class="sxs-lookup"><span data-stu-id="8ab77-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="8ab77-110">若要打开“Azure 信息保护”边栏选项卡，你必须具有 [Azure 信息保护高级计划](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)或包含权限管理的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="8ab77-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="8ab77-111">如果你拥有其中一个订阅，但看到“找不到有效订阅”的消息，请[联系 Microsoft 支持部门](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)或使用你的标准支持频道。</span><span class="sxs-lookup"><span data-stu-id="8ab77-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="8ab77-112">找到“**管理**”菜单选项，然后选择“**保护激活**”。</span><span class="sxs-lookup"><span data-stu-id="8ab77-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="8ab77-113">单击“**激活**”，然后确认你的操作。</span><span class="sxs-lookup"><span data-stu-id="8ab77-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="8ab77-114">激活完成后，信息栏将显示“**激活已成功完成**”。</span><span class="sxs-lookup"><span data-stu-id="8ab77-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="8ab77-115">**将“Azure 信息保护”标签迁移到 Office 365 安全与合规中心**</span><span class="sxs-lookup"><span data-stu-id="8ab77-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="8ab77-116">请确保以具有全局管理员权限的用户身份登录。</span><span class="sxs-lookup"><span data-stu-id="8ab77-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="8ab77-117">导航到“**Azure 信息保护**”边栏选项卡。</span><span class="sxs-lookup"><span data-stu-id="8ab77-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="8ab77-118">从“**管理**”菜单选项中，选择“**统一标签**”。</span><span class="sxs-lookup"><span data-stu-id="8ab77-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="8ab77-119">在“**Azure 信息保护 - 统一标签**”边栏选项卡上，单击“**激活**”并按照联机说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="8ab77-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="8ab77-120">**注意**：在激活安全与合规中心迁移之前，请验证你是否具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="8ab77-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="8ab77-121">请参阅以下文章了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="8ab77-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="8ab77-122">是否必须是全局管理员才能配置 Azure 信息保护，或者我是否可以将此工作委派给其他管理员？</span><span class="sxs-lookup"><span data-stu-id="8ab77-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="8ab77-123">有关迁移到安全与合规中心后的管理角色的重要信息。</span><span class="sxs-lookup"><span data-stu-id="8ab77-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="8ab77-124">有关安全与合规中心中的 AIP 到统一标签迁移的详细信息，请参阅[迁移标签](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)。</span><span class="sxs-lookup"><span data-stu-id="8ab77-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
