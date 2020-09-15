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
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>在合规中心从 AIP 迁移到 MIP/统一标签

若要在安全与合规中心从 AIP 标签迁移到统一标签，请执行下列操作：

**从 Azure 门户激活保护**

1. 如果尚未执行此操作，请打开一个新的浏览器窗口，然后[登录 Azure 门户](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)。 导航到“**Azure 信息保护**”边栏选项卡。 例如，在中心菜单上，单击“**所有服务**”并开始在“筛选器”框中键入**信息**。 选择“**Azure 信息保护**”。 如果之前未访问过“Azure 信息保护”边栏选项卡，请参阅一次性[其他步骤](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)，将此边栏选项卡添加到门户。 若要打开“Azure 信息保护”边栏选项卡，你必须具有 [Azure 信息保护高级计划](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)或包含权限管理的 Office 365 计划。 如果你拥有其中一个订阅，但看到“找不到有效订阅”的消息，请[联系 Microsoft 支持部门](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)或使用你的标准支持频道。

2. 找到“**管理**”菜单选项，然后选择“**保护激活**”。 单击“**激活**”，然后确认你的操作。 激活完成后，信息栏将显示“**激活已成功完成**”。

**将“Azure 信息保护”标签迁移到 Office 365 安全与合规中心**

1. 请确保以具有全局管理员权限的用户身份登录。

2. 导航到“**Azure 信息保护**”边栏选项卡。

3. 从“**管理**”菜单选项中，选择“**统一标签**”。

4. 在“**Azure 信息保护 - 统一标签**”边栏选项卡上，单击“**激活**”并按照联机说明进行操作。

**注意**：在激活安全与合规中心迁移之前，请验证你是否具有相应的权限。 请参阅以下文章了解详细信息：

1. [是否必须是全局管理员才能配置 Azure 信息保护，或者我是否可以将此工作委派给其他管理员？](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [有关迁移到安全与合规中心后的管理角色的重要信息。](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

有关安全与合规中心中的 AIP 到统一标签迁移的详细信息，请参阅[迁移标签](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)。
