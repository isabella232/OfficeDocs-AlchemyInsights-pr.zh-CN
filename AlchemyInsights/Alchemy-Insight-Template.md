---
title: 与文件名相同是最佳
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312815"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"必需 Alchemy Header H1， H2's don's don't work."
有关 Alchemy 创作的最佳实践和指南：

1. **不要将 Alchemy Insights嵌套在文件夹中**- 这将破坏 url 结构。 我们正在寻找解决此问题的考虑。
1. **AlchemyInsights** 文件夹中的文件应包含小写文件名以及空格（例如）的连字符。 **_how-to-enable-litigation-hold_**.
    1. 在 ms.custom 字段中包括 [Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net) 中的规则 ID 或存储桶 ID。 例如， ***ms.custom： 100021***
1. 将此文件顶部的其余元数据用作模板。
1. 在 ["Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net)"中，导航到"客户见解标题 **："** 部分，并使用它作为了解的 H1 标题的起点。 

**注意**：Insights在顶部只能有一个 H1，否则将在生产中中断。 H2 不会呈现，因此请使用 **粗体** 或其他约定来表示单独的部分。
1. 接下来，使用"Alchemy 规则"页的"Customer Insights"部分中的草稿材料填写正文文本
    1. 项目符号列表正常
    1. 编号列表也
    1. **粗体***和 italic* 表示正常
    1. 链接应始终为"Web **链接"/指向** **UI** 元素的外部或深层链接，而不是内部链接。
    1. 目前，图片不受正式支持，但已制定路线图。

这实际上有点过长。 最佳做法是大约 400 个字符---------------------------------

内容准备就绪后，将其拉至活动分支。 然后，转到 ["Alchemy 合作伙伴门户](https://alchemyportal.azurewebsites.net) "，在 url 字段中输入文件名。 