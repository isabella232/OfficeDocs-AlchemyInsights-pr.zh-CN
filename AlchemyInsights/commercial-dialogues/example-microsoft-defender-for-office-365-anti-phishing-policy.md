---
title: Microsoft Defender Office 365防钓鱼策略的示例
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034996"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defender Office 365防钓鱼策略的示例

这些设置启用名为域和 *CEO 的策略*。 此策略提供用户和域保护，防止模拟，然后将该策略应用于域中用户接收的所有电子邮件。 首先，添加以下信息以创建策略：

- **名称**：域和 **CEO** 说明：确保 CEO 和您的域未被模拟。
  **应用于 ：** 选择 **收件人域为**。 Under **Any of these，** select **Choose**， and then select a domain. 选择“+ 添加”。 选中列表中域名称旁边的复选框，例如 ("contoso.com) "，然后选择"添加 **"。**  选择“完成”。
- 创建策略后，可以使用以下选项微调策略：
  - **添加要保护的用户：** 对于此示例，至少添加 CEO 的电子邮件地址。
  - **添加要保护的域**：添加包含 CEO 办公室的组织域。
  - **选择操作**：如果 **电子邮件** 是由模拟用户发送的，请选择"将邮件重定向到其他电子邮件地址"，然后输入安全管理员的电子邮件地址 (例如，securityadmin@contoso.com *) 。* 对于 **"如果电子邮件由模拟域发送"，请选择**"**隔离邮件"。**
  - **邮箱智能**：默认情况下，此选项是在创建新的防钓鱼策略时选中的。 最好将此设置保留为“打开”。
  - **添加受信任的发件人和域：** 对于此示例，不要定义任何替代。
- 查看设置后，请根据情况选择 **"创建此** 策略"或 **"保存**"。

若要了解更多信息，请参阅 Microsoft 365 中的[反网络钓鱼Microsoft 365。](https://go.microsoft.com/fwlink/?linkid=2092235)
