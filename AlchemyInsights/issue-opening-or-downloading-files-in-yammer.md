---
title: 在 Yammer 中打开或下载文件时遇到问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146762"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>在 Yammer 中打开或下载文件时遇到问题

经典 Yammer 支持将文件上传到消息和组的多个选项。 根据网络配置，文件默认存储在 SharePoint 中。

新版 Yammer 中的文件选取器尚无法支持经典 Yammer 中提供的所有选项。 未来的更新将会添加其他功能。 有关详细信息，请参阅[将文件或图像附加到 Yammer 对话帖子](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)。

**无法打开或下载文件**  

文件可能上传到 Yammer，但同时又链接到 SharePoint Online 中的文件。 若要解决此问题，首先必须确定文件的位置。 如果已将文件上传到 Yammer，则它将具有 *.yammer.com URL。 确保已取消阻止所需 URL 和 IP 地址。 有关详细信息，请参阅博客文章[不建议针对 Yammer 使用硬编码的 IP 地址](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)。

检查某个也是全局管理员身份的用户是否可以下载该文件。 如果文件是专用的，则可能需要使用“专用内容模式”。 有关详细信息，请参 [监视 Yammer 中的专用内容](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)。  

**Yammer 网络级别的来宾和 SharePoint Online 中的文件**  

[Yammer 中的网络级别来宾](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)不使用 Azure AD B2B，并且只能在 Yammer 服务内部活动，因此不能访问存储在 SharePoint 中的 Yammer 文件。 请创建可使用 AAD B2B 标识访问 SharePoint Online 中的文档库的外部 AAD B2B 用户。 有关未来在 Yammer 中提供 Azure AD B2B 来宾支持的详细信息，请参阅[Yammer 预览版中的企业对企业 (B2B) 来宾支持 - 客户条款和常见问题解答](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)。