---
title: 646 如何配置 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277091"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f707c-102">配置同步功能</span><span class="sxs-lookup"><span data-stu-id="f707c-102">Configure sync features</span></span>

<span data-ttu-id="f707c-p101">Azure AD 连接提供了众多功能的默认情况下，启用或更高版本可以启用。某些功能需要特定环境中的其他配置。</span><span class="sxs-lookup"><span data-stu-id="f707c-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="f707c-p102">[筛选](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制对象同步到 Azure AD。默认情况下，所有用户、 联系人、 组和 Windows 10 都同步计算机帐户。您可以包括或排除基于域、 Ou、 或其他属性的对象。</span><span class="sxs-lookup"><span data-stu-id="f707c-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="f707c-p103">[密码哈希同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)同步从内部部署 Active Directory 密码哈希与 Azure AD。这将允许密码管理在一个位置，但相同密码中同时使用内部部署和云环境。由于 Active Directory 的权威源，您可以使用您自己的密码策略。</span><span class="sxs-lookup"><span data-stu-id="f707c-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="f707c-111">[自助服务密码重置 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允许用户仍将应用您的本地密码策略时重置云中自己的密码。</span><span class="sxs-lookup"><span data-stu-id="f707c-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="f707c-112">[设备写回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允许 Azure AD 以便它们可用于条件的访问，重新写入到内部部署 Active Directory 中注册的设备。</span><span class="sxs-lookup"><span data-stu-id="f707c-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="f707c-p104">[防止意外删除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)默认情况下启用为了帮助防止太多同时对象删除 （每个同步多于 500 个对象）。您可以更改此设置以满足组织的需求。</span><span class="sxs-lookup"><span data-stu-id="f707c-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="f707c-115">对于 express 安装默认情况下启用[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)并有助于确保您的 Azure AD 连接版本始终是最新。</span><span class="sxs-lookup"><span data-stu-id="f707c-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

