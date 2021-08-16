---
title: Yammer 中的通知
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097188"
---
# <a name="notifications-in-yammer"></a>Yammer 中的通知

若要向你提醒相关对话中的新活动，Yammer 会通过电子邮件[向你发送通知](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)，如果你是在移动设备上使用 Yammer，则会通过推送通知进行提醒。 默认情况下，Yammer 会向你发送所在网络中各种类型活动的通知。 用户可以通过 Yammer 网站更新其电子邮件设置，通过移动应用配置推送通知。 

Yammer 添加了[对 Outlook 中的交互式电子邮件](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420)的支持。 某些电子邮件（邮件副本）将在 Outlook 网页版中具有交互性。 在以后的更新中，其他版本的 Outlook 也将具备此功能。

**Yammer 中的通知类型**

- 电子邮件（来自组的最新动态、他人向你发出的入组邀请、你的收件箱中收到邮件等）
- 推送通知（在提到你以及收件箱收到邮件等时候向移动设备发送的通知）
- 桌面弹出窗口（安装 Yammer 桌面应用后，该应用会向用户显示名为“Toast”的通知。）
- 铃声通知（用户可以在 Yammer 网站内看到针对不同事件的通知。 这些通知可能并非总是有对应的电子邮件或推送通知。）

请参阅我们提供的[有关通知的详细信息](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)。

**管理通知**

用户必须管理自己的通知。 请参阅有关[如何启用和禁用 Yammer 电子邮件和手机通知](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)的信息。 

管理员不可能代表用户禁用所有通知，或代表用户控制通知。 管理员可以[控制电子邮件中包含的徽标，以及用户是否需要确认通过电子邮件](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer)发送的邮件。

**向组织中的多个用户发送电子邮件通知**

有时，Yammer 发出的单个电子邮件通知会被组织中的许多用户收到，其数量超出预想。 在将通讯组列表或其他类型的非个人电子邮件地址添加到 Yammer 时，就会发生这种情况。 Yammer 并不总是知道这些电子邮件地址是属于个人用户，还是会造成一封电子邮件发送给许多收件人的电子邮件地址。 发生此问题时，你必须采取措施，在 Yammer 中[挂起（停用）具有该电子邮件地址的无效用户](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。 

若要减少发生此问题的机率，请执行以下操作：

1. [强制使用适用于 Yammer 用户的 Office 365 标识](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。
2. 阻止外部发件人向你的组织发送电子邮件，或限制为只有获得批准的用户可以发送电子邮件。

如果出现此问题：

1. 确定电子邮件的收件人，其应与 Yammer 中的用户匹配。 例如，all-in-sales@fabrikam.com 是一个 DL，适用于所有销售人员。 此 DL 可以从用户收到的 Yammer 电子邮件识别出来。
2. 使用[“网络管理员”中的停用（挂起）功能](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)来挂起具有 all-in-sales@fabrikam.com 电子邮件地址的用户。 挂起可以撤消，因此比删除更安全。 该用户将在 90 天后被自动删除。
3. 此外还可以选择查看“[用户导出](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers)”来发现其他应该被挂起的非用户电子邮件地址。
