---
title: 在"应用注册"边栏选项卡上查找缺少的应用程序
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
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057092"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>在"应用注册"边栏选项卡上查找缺少的应用程序

1. 无法在应用注册门户上找到应用程序。

    如果应用程序是多租户应用程序，并且已在另一个租户中注册，它将不会显示在"应用注册"边栏选项卡下。 但是，在租户Enterprise创建服务主体 (后，你可能会在"Enterprise) 应用程序"边栏选项卡下找到它。 有关详细信息，请参阅[应用& Azure AD 中的](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)服务主体 - Microsoft 标识平台。
2. 即使你是管理员，也无法在"应用注册"边栏选项卡中查看应用。

    请确保你位于 Azure 门户上的正确目录中。
3. 我的应用程序未列在"Enterprise应用程序"边栏选项卡下，但在我查询 PowerShell 命令时它将显示。

    有时，从 Azure 门户删除应用程序后，它不会显示在门户中，但可能尚未完全删除。 有关详细信息，请参阅：
    - 可以使用 Powershell 命令 **（Get-AzureADDeletedApplication）** 检索以前删除的应用程序的列表，并查看该应用程序是否显示在列表中。 若要了解更多信息，请参阅 [Get-AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)。
    - 如果你想要完全删除应用程序，可以在 PowerShell 中尝试以下操作 **：Remove-AzureADApplication -ObjectId**。 若要了解更多信息，请参阅 [Remove-AzureADApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)。
    - 或者，可以尝试使用以下 Powershell 命令还原已删除的应用程序： **还原 AzureADDeletedApplication -ObjectId**。 若要了解更多信息，请参阅 [Restore-AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)。
4. 找不到新 Azure 租户中所有预安装的企业应用程序的列表。

    Azure AD 中默认没有预安装的企业应用程序。 你需要通过从 Azure AD 库浏览它或添加非库应用程序，从"新建应用程序"选项手动添加它。 若要了解更多信息，请参阅[快速入门：将应用程序添加到 Azure AD Azure Active Directory (租户) 应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)。
    如果你是全局管理员，可以使用"应用"Microsoft 365[轻松](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)Launcher。
5. 无法从"我的应用程序"门户找到我的应用程序。

    确保应用程序未在"我的应用程序"集合页中隐藏。 若要了解更多信息，请参阅"我的 ([Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)) 中的"集合"和预览版。
6. 若要从"我的应用"门户启动应用，请参阅在"我的& [- Azure AD"](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)上找到"使用应用"。
7. Office 365安装后，Mover 应用不会显示在Enterprise应用程序边栏选项卡上。

    "Office 365 Mover"应用程序是一个多租户应用，无需使用"应用注册"下的"库应用程序"部分Enterprise AAD。 若要Office 365 Mover 应用，只需登录该应用，它将请求用户同意权限。 在用户同意后，此应用程序将自动添加到具有已登录的电子邮件 ID 的租户。

    登录应用程序后，你应该能够在 AAD 中的 Enterprise Applications 边栏选项卡下找到此应用程序的条目。 你需要通过键入全名（例如"Office 365 Mover"或仅搜索"office"来搜索该应用程序，它应列出该应用。 若要了解更多信息[，Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)表示它已安装，但它未在 Enterprise 应用程序库中列出。
8. 快速入门：查看使用[Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)租户进行身份管理的应用程序列表将展示如何查看已设置为将 Azure AD 租户用作其标识提供程序 (IdP) 的应用程序（也称为应用）。
9. [解决向应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps)中添加或删除应用程序的常见问题Azure Active Directory有助于了解用户查看应用程序中的应用时Azure Active Directory。
