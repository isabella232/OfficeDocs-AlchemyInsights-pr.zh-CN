---
title: 646如何配置 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722517"
---
# <a name="configure-sync-features"></a><span data-ttu-id="d1ed5-102">配置同步功能</span><span class="sxs-lookup"><span data-stu-id="d1ed5-102">Configure sync features</span></span>

<span data-ttu-id="d1ed5-103">Azure AD Connect 包括在默认情况下启用的几项功能，或者您可以稍后启用的功能。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="d1ed5-104">某些功能需要在特定环境中进行额外配置。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="d1ed5-105">[筛选](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制将对象同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="d1ed5-106">默认情况下，将同步所有用户、联系人、组和 Windows 10 计算机帐户。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="d1ed5-107">您可以基于域、Ou 或其他属性包含或排除对象。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="d1ed5-108">[密码哈希同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)将密码哈希从本地 Active Directory 同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="d1ed5-109">这将允许在一个位置进行密码管理，但在本地和云环境中使用相同的密码。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="d1ed5-110">由于 Active Directory 是权威源，因此您可以使用自己的密码策略。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="d1ed5-111">[自助密码重置（SSPR）](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允许用户在应用本地密码策略的同时在云中重置自己的密码。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="d1ed5-112">[设备写回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允许 Azure AD 中的注册设备被写回本地 Active Directory，以便它们可用于条件访问。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="d1ed5-113">默认情况下，将启用[意外删除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)以帮助防止同时删除的对象过多（每个同步有500个以上的对象）。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="d1ed5-114">您可以更改此设置以满足组织的需求。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="d1ed5-115">默认情况下会为 express 安装启用[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)，并有助于确保你的 Azure AD Connect 版本始终是最新的。</span><span class="sxs-lookup"><span data-stu-id="d1ed5-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
