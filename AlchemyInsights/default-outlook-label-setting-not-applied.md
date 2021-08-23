---
title: 默认Outlook未应用标签设置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370208"
---
# <a name="default-outlook-label-setting-not-applied"></a>默认Outlook未应用标签设置

如果您的 Outlook默认标签设置未正确应用，并且未应用其他标签或未应用标签，则可能会遇到已知问题 (MC277818) 并且应执行以下两个选项之一来解决问题：

**选项 1：**

1. 转到"Microsoft 365合规中心>**解决方案**  >  **信息保护"。**
1. 选择 **"标签** 策略"，然后选择编辑所需的标签策略 (在相关标签策略上未正确设置 **OutlookDefaultlabel** 设置。 运行 **Get-labelpolicy** 以查看此设置) ，然后选择"编辑 **策略"。**
1. 选择 **"** 下一步"，直到在"策略设置"对话框中选择"要求用户向电子邮件和文档应用标签"设置"，才能看到"向电子邮件应用此默认 **标签"设置**。
1. 在" **将默认标签应用于文档** "对话框中 **，从下拉列表** 中选择"无"。
1. 选择 **"下** 一 **步"** 和"提交"以保存标签设置。

**选项 2：**

在 [安全与](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)合规中心 Powershell 中，使用 Set-LabelPolicy 命令将 **{OutlookDefaultLabel="None"} 上的 OutlookDefaultlabel** 更改为 **None。**

运行： `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

有关用户的默认标签Outlook，请参阅设置其他[默认标签Outlook。](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)