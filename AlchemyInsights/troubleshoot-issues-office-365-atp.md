---
title: 解决 Office 365 高级威胁防护（ATP）的问题
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766735"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>解决 Office 365 ATP 中的问题

- **注意电子邮件传递是否延迟**？ 尝试对 ATP 安全附件策略使用动态传递选项。 这将避免电子邮件传递延迟，同时防止收件人受到恶意文件的攻击。
- **是否要报告误报或漏报**？ 使用此链接提交您的文件以供分析：[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **您是否知道您可以为组织中的人员发送的电子邮件启用 ATP 安全链接保护**？ 请按以下步骤操作：
    1. 转到https://protection.office.com，然后登录。
    2. 转到 "**威胁管理** > **策略** > **安全链接**"。
    3. 在 "**适用于特定收件人的策略**" 下，编辑（或添加）策略。
    4. 选择 "**将安全链接应用于在组织内发送的邮件"**。
    5. 保存您的策略，并大约等待30分钟，以使更改在您的数据中心中工作。
- 若要获取有关 ATP 的更多帮助，请参阅[Office 365 高级威胁防护](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)。