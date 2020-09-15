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
ms.openlocfilehash: 233354386eb319860f25b3929b6be528438cc865
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680413"
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
