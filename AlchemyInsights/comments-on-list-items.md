---
title: 对列表项的注释
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995467"
---
# <a name="comments-on-list-items"></a>对列表项的注释

用户可以查看列表项上的所有注释，并可在显示与项目相关的注释或活动的视图之间筛选。

用户需要先注意以下事项，然后才能添加和删除注释：

- 注释遵循自定义权限中固有的SharePoint。
- 尚未构建以显示在新式用户界面（如任务列表）中的经典列表将没有此注释功能。
- 此版本未提供Teams中的列表注释功能。
- 搜索不会对注释编制索引。

管理员可以在组织级别禁用此功能，方法为更改 **Set-SPOTenant** PowerShell cmdlet 中的 **CommentsOnListItemsDisabled** 参数。

当前不可能在站点或列表级别禁用注释。 我们希望在 2021 年第一季度的更新中提供这些控件。
