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
# <a name="configure-service-connection-point-scp"></a>配置服务连接点 (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED （0x801c001d/-2145648611）**

- **原因**：无法读取 SCP 对象并获取 Azure AD 租户信息
- **解决方案**：请参阅 [ 配置服务连接点](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**操作计划**

- 检查设备是否已接收用于控制验证的 GPO。
- 确保 GPO 已创建注册表项。
- 确保有 2 个 用目录ID和 onmicrosoft 域创建的密钥。

**配置SCP的客户端注册表设置** 

使用以下示例创建组策略对象(GPO)来部署注册表设置，该设置在设备的注册表中配置 SCP 条目。

1. 打开组策略管理控制台，在域中创建新的 GPO。
     - 为新创建的 GPO 提供名称（例如 ClientSideSCP）

2. 编辑 GPO 并找到以下路径： **"计算机配置">"首选项">"Windows 设置">"注册表**。

3. 右键单击 **注册表** ， **"新建">"注册表项**。

4. 在 **“常规”** 选项卡上，配置下列设置：
  
- **操作**：更新
    
- **配置单元**: HKEY_LOCAL_MACHINE
    
- **键路径**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **值名称**：TenantId
    
- **值类型**：REG_SZ
    
- **值数据**：Azure AD 实例的 GUID 或目录 ID（可在 **Azure 门户 >Azure Active Directory >"属性">"目录 ID**）
 
- 单击“**确定**”。
 
5. 右键单击 **注册表** ， **"新建">"注册表项**。

6. 在 **“常规”** 选项卡上，配置下列设置：
  
- **操作**：更新
    
- **配置单元**: HKEY_LOCAL_MACHINE
    
- **键路径**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **值名称**：TenantName
    
- **值类型**：REG_SZ
    
- **值数据**：使用联合环境 (如 AD FS) 时已验证的域名。 已验证域名或你的 onmicrosoft.com 域名（例如，contoso.onmicrosoft.com，如果使用的是托管环境）

- 单击“**确定**”。

7. 关闭新创建 GPO 的编辑器。

8. 将新创建的 GPO 链接到所需的 OU，该 OU 包含属于受控推出群体的域连接计算机。

有关详细信息，请参阅 [混合 Azure AD 联接受控验证 - Azure AD |Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Azure Active Directory 加入的设备的疑难解答|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)。









