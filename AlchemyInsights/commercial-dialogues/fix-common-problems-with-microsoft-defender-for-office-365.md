---
title: 修复 Microsoft Defender for Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330050"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>修复 Microsoft Defender for Office 365

以下是 Microsoft Defender for Office 365 的常见问题的一Office 365：

- **邮件延迟**：

  电子邮件传递延迟可能是由邮件保险箱附件扫描导致。 有关详细信息，请参阅附件[保险箱设置](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)。

- **报告误报或负结果**：

  有关详细信息，请参见[向 Microsoft 报告邮件和文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)。

- **启用保险箱链接保护**：

  1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> ， go to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **保险箱 Links** in the **Policies** section.

     若要直接转到"链接 **保险箱，** 请使用 <https://security.microsoft.com/safelinksv2> 。

  2. On the **保险箱 Links** page， select the policy by clicking on the name of the policy.
  3. 在出现的详细信息飞出中，执行下列任一步骤：
     - 若要添加新策略，请选择" **+ 创建"。** 向导将启动，帮助你定义策略设置。
     - 若要编辑现有策略，请通过单击该策略的名称来选择该策略。 在出现的详细信息飞出控件中，选择"保护设置 **"****部分中的"编辑**"。
  4. 在" **保护设置"** 页上，配置以下设置：
     - 打开 选择 **邮件中未知潜在恶意 URL 的操作**。
     - 选择 **"将安全链接应用于在组织内部发送的邮件"。**

  有关详细信息，请参阅在[Microsoft Defender 保险箱设置链接策略Office 365。](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
