---
title: 启用 Azure AD Connect 中的密码写回
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
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709717"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>启用 Azure AD Connect 中的密码写回

若要启用自助服务密码重置写回，请首先在 Azure AD Connect 中启用写回选项。 在 Azure AD Connect 服务器中，完成以下步骤：

1. 登录 Azure AD Connect 服务器，然后启动 **Azure AD Connect** 配置向导。
2. 在“**欢迎**”页上，单击“**配置**”。
3. 在“**其他任务**”页上，选择“**自定义同步选项**”，然后单击“**下一步**”。
4. 在“**连接到 Azure AD**”页面上，输入全局管理员凭据，然后单击“下一步”。
5. 在“**连接到目录**”和“**域/OU**”筛选页上，单击“**下一步**”。
6. 在“**可选功能**”页上，选中“**密码写回**”旁边的框，然后单击“**下一步**”。
7. 在“**准备配置**”页上，单击“**配置**”并等待该过程完成。
8. 当看到配置完成后，单击“**退出**”。

在 Azure AD Connect 中启用密码写回后，现在配置用于写回的 Azure AD SSPR。  若要在 SSPR 中启用密码写回，请完成以下步骤：

1. 使用全局管理员帐户登录到 Azure 门户。
2. 搜索并选择 **Azure Active Directory**，单击“**密码重置**”，然后选择“**本地集成**”。
3. 把选项“**将密码回写到本地目录？**”设置为“**是**”。
4. 将“**允许用户在不重置密码的情况下解锁帐户**”选项设置为“**是**”。
5. 准备好后，单击“**保存**”。

有关详细信息，请参阅“[对本地环境启用 Azure Active Directory 自助服务密码重置写回](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)”。
