---
title: 推迟 Windows 10 更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1128"
- "6700007"
ms.openlocfilehash: 18a73fdb5a0b270b4343c408ef97fb18388b629bec63fc59fdfa674b763369be
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118554"
---
# <a name="defer-windows-10-updates"></a>推迟 Windows 10 更新

若要推迟推送给用户的 Windows 10 更新，请按照以下步骤操作：

1. 登录 Azure 门户。
2. 选择“**软件更新**”  >  “**Windows 10 更新通道**”。
3. 如果没有更新通道，请选择相关选项来新建一个。
4. 输入名称和可选说明，然后选择“**设置配置**”。
5. 自定义推迟不同更新的时间范围。 最大推迟时间基于更新类型：
    - **质量更新** - 自发布之日起，最长可推迟 30 天。
    - **功能更新** - 自发布之日起，最长可推迟 180 天。
