---
title: 支持嵌入旧版对话框以打开报告
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
- "9002931"
- "5612"
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003379"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>支持嵌入旧版对话框以打开报告

**症状**

用户无法打开报告。 “出现错误。 请查看技术详细信息获取更多信息。”

**原因**

无法在 UCI 中加载报告，并显示错误“表单描述符为 NULL 或未定义”。 UCI 中的报告仍然需要旧版对话框，因此客户系统需要启用 *allowacyacydialogsemdding*。

**解决方案**

1. 转到 **“设置”>“管理”>“系统设置”>“常规”** 选项卡。

2. 将“支持在统一界面浏览器客户端中嵌入某些旧版对话框”设置为“**是**”。
