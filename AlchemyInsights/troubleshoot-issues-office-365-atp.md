---
title: '解决 Office 365 中的问题高级威胁防护 (ATP) '
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758055"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>解决 Office 365 ATP 中的问题

- **注意电子邮件传递是否延迟**？ 尝试对 ATP 安全附件策略使用动态传递选项。 这将避免电子邮件传递延迟，同时防止收件人受到恶意文件的攻击。
- **是否要报告误报或漏报**？ 使用此链接提交您的文件以供分析： [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **您是否知道您可以为组织中的人员发送的电子邮件启用 ATP 安全链接保护**？ 请按以下步骤操作：
    1. 转到 https://protection.office.com ，然后登录。
    2. 转到 "**威胁管理**  >  **策略**  >  **安全链接**"。
    3. 在 " **适用于特定收件人的策略**" 下，编辑 (或添加) 策略。
    4. 选择 " **将安全链接应用于在组织内发送的邮件"**。
    5. 保存您的策略，并大约等待30分钟，以使更改在您的数据中心中工作。
- 若要获取有关 ATP 的更多帮助，请参阅 [Office 365 高级威胁防护](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)。