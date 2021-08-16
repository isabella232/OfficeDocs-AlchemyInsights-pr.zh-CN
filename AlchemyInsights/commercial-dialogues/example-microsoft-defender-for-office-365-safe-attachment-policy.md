---
title: Microsoft Defender for Office 365 保险箱 附件策略示例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988285"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Microsoft Defender for Office 365 保险箱 附件策略示例

这些设置启用名为 *"无延迟* "的策略，该策略可立即传递邮件，然后在扫描附件后重新附加附件：

- **名称**：无延迟
- **说明**：立即传递邮件，在扫描后重新附加附件。
- **响应**：选择 **"动态传递"** 选项。 有关详细信息，请参阅动态[传递保险箱附件策略。](https://go.microsoft.com/fwlink/?linkid=2092328)
- **重定向附件** 部分：选择"启用重定向"选项，然后输入将调查恶意附件的 Microsoft 365 全局管理员、安全管理员或安全分析师的电子邮件地址。
- **"应用于** "部分： **选择"收件人域是**"，然后选择您的域。 选择 **"添加**"，然后选择"确定 **"。** 完成后，选择 **保存。**

若要了解更多信息，请参阅[保险箱 Microsoft Defender 中的附件Office 365。](https://go.microsoft.com/fwlink/?linkid=2092213)
