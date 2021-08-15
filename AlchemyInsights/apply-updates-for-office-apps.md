---
title: 应用 Office 更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969375"
---
# <a name="apply-updates-for-office-apps"></a>应用 Office 更新

默认情况下，Office Apps 的更新是免费的，可自动下载并在后台应用，无需用户进行任何干预。 如果在应用更新时遇到问题，要手动运行更新，请参阅[安装 Office 更新](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)。 有关详细信息，请参阅 [安装 Office 的疑难解答](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)。

若要为用户管理 Office 更新，请考虑以下选项：

- 根据所需的更新频率为你的组织选择合适的 Office 更新通道。 若要了解如何操作，请参阅 [Microsoft 365 应用版的更新通道概述](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)。

- 决定是自动从 internet 还是从本地共享应用更新。 若要了解如何操作，[选择如何管理 Microsoft 365 应用版的更新](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)。

- 查看 Office 更新设置以控制如何将更新应用于最终用户计算机：

    - [配置 Microsoft 365 应用版的更新设置](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)。
    - [定义如何在安装后更新 Office](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)。

将 Office 应用部署到多个用户时，请使用 Office 自定义工具构建用于部署的配置文件，并使用 Office 部署工具配置 Office 更新。 有关详细信息，请参阅 [Office 自定义工具概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)和 [Office 部署工具](https://go.microsoft.com/fwlink/p/?LinkID=626065)。

- 有关如何设置用户组以部署 Office 更新的示例，请参阅[从本地源部署 Microsoft 365 应用版](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)。
-   如果因为打开 Office 应用，Office 更新未应用于少数用户，请考虑使用 ForceAppShutdown 设置。 有关更多信息，请参见[FORCEAPPSHUTDOWN 属性（Property 元素的一部分）](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)。 

**另请参阅**

[Microsoft 365 应用版更新过程概述](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)。  
[Microsoft 365 应用版更新发行信息](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)。  
[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 应用版更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)。  
