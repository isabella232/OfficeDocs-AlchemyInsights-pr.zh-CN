---
title: 登录到OneDrive的故障排除
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: fb944ae8dac7a8a222d2946025d8009216d6ca02efa750977bc9037bf578c8a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972598"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>登录到OneDrive的故障排除

本文介绍了以下方案：

- 解决有关登录OneDrive同步客户端的问题
- 解决有关登录 OneDrive for Business 网站的问题

**解决有关登录 OneDrive 同步客户端的问题**

- 有关解决错误代码 0x004de40 的信息，请参阅 [登录 OneDrive 时遇到错误代码 0x8004de40](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive)。
- 通过访问OneDrive或SharePoint网站登录，然后点击网站菜单栏顶部的 **同步** 按钮。
- 确保正在登录OneDrive for Business，而不是OneDrive.com。 如果访问的 URL 以 onedrive.live.com 开头，则不是 OneDrive for Business 的位置。 确保你登录OneDrive for Business的简单方法是通过这个链接：https://portal.office.com/onedrive 然后使用工作或学校帐户登录。
- 如果仍然遇到问题，请考虑[充值OneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)。
- [取消帐户与 OneDrive 的链接](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)，登录到 OneDrive 或 SharePoint 网站，然后单击网站上菜单栏顶部的 **同步** 按钮。

**解决有关登录 OneDrive for Business 网站的问题**

- 确保正在登录OneDrive for Business，而不是OneDrive.com。 如果访问的 URL 以 onedrive.live.com 开头，则不是 OneDrive for Business 的位置。 确保你登录OneDrive for Business的简单方法是通过这个链接：https://portal.office.com/onedrive 然后使用工作或学校帐户登录。
- 如果重定向到Delve配置文件页面，Microsoft 365管理员将需要[授予用户创建其OneDrive for Business站点的权利 ](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)。
- 通过使用[Microsoft Edge中的InPrivate浏览](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc)（或其他浏览器中的类似功能）来测试是否可以访问OneDrive网站。
    - 如果 InPrivate 浏览有效，可能需要[清楚Microsoft Edge](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4)中的浏览数据（或其他浏览器中的类似功能）。

**登录Office与OneDrive同步的故障排除**

如果你得到一个错误信息说 **上传受阻**，**登录到保存这个文件**，或 **保存副本**，可能需要 [删除并从Office连接服务中重新连接OneDrive](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)。

**其他疑难解答提示**

如果你是全局、许可证或用户管理员，[请将正确的许可证分配给受影响的用户](/microsoft-365/admin/manage/assign-licenses-to-users)。

