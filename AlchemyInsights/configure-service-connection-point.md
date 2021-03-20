---
title: 配置服务连接点 (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897545"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="f0f2d-102">配置服务连接点 (SCP)</span><span class="sxs-lookup"><span data-stu-id="f0f2d-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="f0f2d-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED （0x801c001d/-2145648611）**</span><span class="sxs-lookup"><span data-stu-id="f0f2d-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="f0f2d-104">**原因**：无法读取 SCP 对象并获取 Azure AD 租户信息</span><span class="sxs-lookup"><span data-stu-id="f0f2d-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="f0f2d-105">**解决方案**：请参阅 [ 配置服务连接点](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="f0f2d-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="f0f2d-106">**操作计划**</span><span class="sxs-lookup"><span data-stu-id="f0f2d-106">**Action plan**</span></span>

- <span data-ttu-id="f0f2d-107">检查设备是否已接收用于控制验证的 GPO。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="f0f2d-108">确保 GPO 已创建注册表项。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="f0f2d-109">确保有 2 个 用目录ID和 onmicrosoft 域创建的密钥。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="f0f2d-110">**配置SCP的客户端注册表设置** </span><span class="sxs-lookup"><span data-stu-id="f0f2d-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="f0f2d-111">使用以下示例创建组策略对象(GPO)来部署注册表设置，该设置在设备的注册表中配置 SCP 条目。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="f0f2d-112">打开组策略管理控制台，在域中创建新的 GPO。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="f0f2d-113">为新创建的 GPO 提供名称（例如 ClientSideSCP）</span><span class="sxs-lookup"><span data-stu-id="f0f2d-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="f0f2d-114">编辑 GPO 并找到以下路径： **"计算机配置">"首选项">"Windows 设置">"注册表**。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="f0f2d-115">右键单击 **注册表** ， **"新建">"注册表项**。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="f0f2d-116">在 **“常规”** 选项卡上，配置下列设置：</span><span class="sxs-lookup"><span data-stu-id="f0f2d-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="f0f2d-117">**操作**：更新</span><span class="sxs-lookup"><span data-stu-id="f0f2d-117">**Action**: Update</span></span>
    
- <span data-ttu-id="f0f2d-118">**配置单元**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="f0f2d-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="f0f2d-119">**键路径**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="f0f2d-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="f0f2d-120">**值名称**：TenantId</span><span class="sxs-lookup"><span data-stu-id="f0f2d-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="f0f2d-121">**值类型**：REG_SZ</span><span class="sxs-lookup"><span data-stu-id="f0f2d-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="f0f2d-122">**值数据**：Azure AD 实例的 GUID 或目录 ID（可在 **Azure 门户 >Azure Active Directory >"属性">"目录 ID**）</span><span class="sxs-lookup"><span data-stu-id="f0f2d-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="f0f2d-123">单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="f0f2d-124">右键单击 **注册表** ， **"新建">"注册表项**。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="f0f2d-125">在 **“常规”** 选项卡上，配置下列设置：</span><span class="sxs-lookup"><span data-stu-id="f0f2d-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="f0f2d-126">**操作**：更新</span><span class="sxs-lookup"><span data-stu-id="f0f2d-126">**Action**: Update</span></span>
    
- <span data-ttu-id="f0f2d-127">**配置单元**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="f0f2d-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="f0f2d-128">**键路径**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="f0f2d-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="f0f2d-129">**值名称**：TenantName</span><span class="sxs-lookup"><span data-stu-id="f0f2d-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="f0f2d-130">**值类型**：REG_SZ</span><span class="sxs-lookup"><span data-stu-id="f0f2d-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="f0f2d-131">**值数据**：使用联合环境 (如 AD FS) 时已验证的域名。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="f0f2d-132">已验证域名或你的 onmicrosoft.com 域名（例如，contoso.onmicrosoft.com，如果使用的是托管环境）</span><span class="sxs-lookup"><span data-stu-id="f0f2d-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="f0f2d-133">单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-133">Click **OK**.</span></span>

7. <span data-ttu-id="f0f2d-134">关闭新创建 GPO 的编辑器。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="f0f2d-135">将新创建的 GPO 链接到所需的 OU，该 OU 包含属于受控推出群体的域连接计算机。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="f0f2d-136">有关详细信息，请参阅 [混合 Azure AD 联接受控验证 - Azure AD |Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Azure Active Directory 加入的设备的疑难解答|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)。</span><span class="sxs-lookup"><span data-stu-id="f0f2d-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









