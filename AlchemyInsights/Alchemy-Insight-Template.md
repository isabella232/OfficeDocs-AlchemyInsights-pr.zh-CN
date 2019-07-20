---
title: 与 filename 的效果最好
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800035"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>必需 Alchemy 标头 H1, H2's 不起作用。
用于 Alchemy 创作的最佳做法和指南:

1. **不在文件夹中嵌套 Alchemy 见解**-这将断开 url 结构。 我们正在寻求解决此情况的情况。
1. **AlchemyInsights**文件夹中的文件的大小写文件名应带有带空格的连字符 (ex)。 操作***方法-保留 "启用-保留***"。
    1. 将规则 ID 或存储桶 ID 包含在 ms. 自定义域中的[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中。 ex. ***ms. custom: 100021***
1. 将此文件顶部的元数据的其余部分用作模板。
1. 在[Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)中, 向下导航到 "**客户洞察力标题:** " 部分, 并将其用作洞察力的 H1 标题的起始点。 
    > [!NOTE]
    > Alchemy 见解必须在顶部只有一个 H1, 否则它们将在生产中中断。 H2s 不呈现任何内容, 因此使用**粗体**或其他约定表示单独的节。
1. 接下来, 使用 Alchemy 规则页面的 "客户见解" 部分中的草稿材料填写正文文本
    1. 项目符号列表正常
    1. 编号列表
    1. **粗体**和*斜体*为-正常
    1. 链接应始终是 **"web 上的链接"/External**或指向**UI 元素的深层链接**, 而不是内部链接。
    1. 目前尚不支持图片, 但这在路线图中。

这实际上已经是太长了。 最佳实践大约为400个字符---------------------------------

准备好内容后, 将其纳入活动分支。 然后, 转到 " [Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)", 并在 "url" 字段中输入文件名。 