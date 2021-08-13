---
title: 排查 Yammer 中的图像加载问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939225"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>排查 Yammer 中的图像加载问题

当 Yammer 中的照片和文件预览出现问题时，请检查是否所有用户都遇到此问题，它是否发生在移动设备上以及在上传附件时是否可再现，以便进行故障排除。  

**个人资料照片问题**  

如果最终用户通过 Microsoft 365 登录 Yammer，则必须更改其个人资料，包括个人资料照片。 如果不允许用户更新个人资料，则管理员可以为该用户执行更新。 有关详细信息，请参阅[在 Office Delve 中查看和更新个人资料](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)。

有关个人资料编辑的信息（包括个人资料照片），请参阅[更改我的 Yammer 个人资料和设置](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)。 

更新的个人资料照片与个人资料属性的同步方式不同。 用户必须登录才能启动其个人资料照片的同步。 有关信息，请参阅[用户个人资料图片是否会从 Office 365 更新到 Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)。

有关 Yammer 的用户生命周期的信息，请参阅[在 Yammer 用户的整个生命周期中通过 Office 365 对其进行管理](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)。  

有关个人资料图片同步在 Microsoft 365 中如何工作的详细信息，请参阅[有关 Microsoft 365 中的个人资料图片同步的信息](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)。  

**文档预览和图像缩略图问题**  

将文件或图像发布到 Yammer 后，可能不会显示预览，原因如下： 

- 文件已损坏，无法进行处理。
- 该文件最近尚未上传到 SharePoint Online，或者 Yammer 出于其他原因具有无效的元数据。
- 已阻止加载预览图像所需的 URL。
- 发布前，用户已删除文件预览。
- 服务问题已阻止生成预览。

**注意** 链接和文件上传的预览可能会有所不同。 指向 Internet 文件的链接或需要其他身份验证的链接可能无法正确显示。

有关详细信息，请参阅[将文件或图像附加到 Yammer 邮件](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)。 