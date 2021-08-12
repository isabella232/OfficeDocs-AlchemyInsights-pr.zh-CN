---
title: 解决组问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 47f00118a5a4b446b6a3b06f0fc6101d00d11b626eaf249bb6ca962a55f7f4d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939333"
---
# <a name="troubleshoot-group-issues"></a>解决组问题

**我需要将组分配给 Azure AD 角色**

若要将 Azure Active Directory （AD） 组分配给 Azure AD 角色，请执行以下步骤：

1. 创建新组 - 以创建新组：

    a. 使用特权角色管理员或全局管理员权限登录 Azure AD 管理中心。 
    b. 选择 Azure Active Directory >"组">"所有组">"新建组"。 
    c. 创建组。

2. 在组创建期间或在组创建之后将角色分配给组。

    a. 要在创建组时将角色分配给组，请打开可以将 Azure AD 角色分配给组切换按钮，并创建组。
    b. 要在组创建后将角色分配给该组，请导航到新创建的组的“已分配角色”选项卡，然后将角色分配给该组。

**我需要管理分配给 Azure AD 角色的组的成员身份**

1. 为防止提升权限，默认情况下，只有特权角色管理员和全局管理员才能修改分配给角色的组的会员资格。 但是，他们可以选择为这样的组分配所有者并委派此任务。 有关详细信息，请参阅 [组在 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)。
2. 有关在 Azure AD 中向组分配角色的常见问题和疑难解答提示，请参阅 [分配给云组的角色的疑难](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)。

**动态组**

1. 如果找不到内置用户属性，请确保属性位于支持的属性列表中。
2. 如果要查找内置设备属性，请确保该属性位于设备属性列表中 
3. 除了内置的用户和设备属性，还可使用"扩展 [属性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)。 从本地 Windows Server AD 或连接的 SaaS 应用程序同步扩展属性后，属性应显示在规则生成器的下拉列表中。 通过使用 PowerShell 查询用户属性并搜索属性名称，可在目录中找到自定义属性名称。 在规则语法中构建规则时，也可使用这些规则。
4. 确保租户具有相应的许可证。 动态组需要租户拥有 Azure AD P1 Premium 许可证。 可在此处访问 Azure AD 许可证计划 [列表](https://azure.microsoft.com/pricing/details/active-directory/)。 可在此处访问企业移动性 + 安全性 [许可](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)。
5. 确保创建动态组的用户的角色是全局管理员、Intune 管理员、组管理员或用户管理员。
6. 请留出一些时间，以便组进行填充。根据租户的大小，首次填充或规则更改后，组可能需要多达 24 小时进行填充。
7. 有关详细信息，请参阅 [动态组成员身份列表创建基于属性的规则](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)。

**我需要删除组**

1. 可以使用 Azure AD Powershell 模块中的 Remove-AzureADGroup cmdlet 从目录中删除组。
2. 在 Azure AD 中尝试删除同步组之前，请确保已删除所有已分配的许可证以避免错误。
3. 有关删除组的信息，请参阅 [已分配许可证的组时删除](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)。

**我需要还原已删除的组**

1. 如果删除了 Office 365 组，则只能在永久删除前 30 天将其还原。 永久删除后，无法再还原组。 在[此处](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)了解有关还原组。
2. 安全组和通讯组不支持此功能。
3. 请确保你有权还原 Office 365 组。全局管理员、组管理员、用户帐户管理员、Intune 服务管理员、合作伙伴第 1 级或第 2 级支持人员以及组的所有者均可以还原组。
4. 在删除后又还原一个动态组时，该组被视为新组，将根据规则进行填充。此过程可能需要多达 24 小时。
5. 有关还原已删除组的信息，请参阅 在 Azure Active Directory [还原已删除的 Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)。

**组过期策略配置**

1. 仅 Office 365 组支持此功能，不支持安全组和通讯组此功能。
2. 为 Office 365 组配置和使用过期策略需要 Azure AD Premium 许可证。
3. 目前，在租户上只能为 Office 365 组配置一个过期策略。
4. 只有全局管理员、组管理员、用户管理员和组的所有者才能续订组。
5. 如果某个 Office 365 组已过期，则它会被删除，且只能在永久删除发生前 30 天内还原。 永久删除后，无法再还原组。 在[此处](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)了解有关还原组。

**基于活动的自动续订**

SharePoint、Outlook 和 Teams 中的用户活动可触发组自动续订。 在组过期前 35 天检查活动。 如果当前组生命周期内存在活动，将自动续订组，且不会向组所有者发送电子邮件通知。

**已过期组的通知计时**

1. 电子邮件通知在组到期前 30 天、15 天和 1 天向 Office 365 组所有者发送。
2. 首次设置过期时，超过到期时间间隔的任何组均设置为过期前 35 天。
3. 组到期日期基于组的续订日期而不是策略更新日期计算。 如果更新了过期策略，到期日期将不会更改。
4. 有关详细信息，请参阅 [Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) 中的和续订电子邮件 [还原已删除的 Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)。

**创建组的权限**

确保你有权创建新组。 全局管理员可在 Azure 门户或访问面板中禁用组创建。 可能需要管理员来新建组或授予你适当的权限。

1. [在 Azure 门户中创建新组并添加成员](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [在 Powershell MSOnline 中创建组](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [在 Powershell 中禁用组创建](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [管理可在 Office 365 中创建组的成员](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [通过 Powershell 禁用 Office 365 欢迎通知](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD 管理角色](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**管理组创建权限**

1. 全局管理员可通过设置 **用户可以在 Azure 门户** 或 **中创建的安全组或 Office 365 组来管理在 Azure 门户或访问面板中创建的 Office 365 组创建安全组。用户可在 Azure 门户中的** 设置中、"**所有组">"常规（设置）"** 中创建 Office 365 组。
2. 如果拥有 Azure AD P1 Premium 许可证，还可限制组创建，以选择一组用户。

**禁用对 Office 365 组的新成员的欢迎通知**

通过向添加到 Office 365 组的用户发送的欢迎通知，可在 Powershell 中将 `UnifiedGroupWelcomeMessageEnabled` 设置为 **False** 禁用。 在此处了解有关此设置 [，](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)。













