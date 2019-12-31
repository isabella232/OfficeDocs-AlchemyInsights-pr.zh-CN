---
title: Bitlocker 恢复密钥
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908805"
---
# <a name="accessing-bitlocker-recovery-keys"></a>访问 Bitlocker 恢复密钥

配置 Bitlocker 设置 Intune Endpoint Protection 策略时，可以定义 Bitlocker 恢复信息是否应存储在 Azure Active Directory 中。

如果配置了该设置，则在 Intune 设备边栏中的设备记录数据中，存储的恢复数据应以两种方式显示为 Intune 管理员：

设备-Azure AD 设备-> "设备" 或 "设备"-> 所有设备-> "设备"-> 恢复密钥

或者，如果有对设备本身的管理访问权限，则可以通过在提升的命令提示符处运行以下命令来查看恢复密钥（密码）：

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
如果在 Intune 中的 enrolment 之前加密了设备，则恢复密钥可能与在 OOBE 过程中用于登录设备的 "Microsoft 帐户" （MSA）相关联。 如果是这样，则使用该https://onedrive.live.com/recoverykey MSA 访问和登录时应显示已存储恢复密钥的设备。
 
如果由于通过基于域的组策略配置而使设备被加密，则恢复信息可能存储在本地 Active Directory 中。
 

