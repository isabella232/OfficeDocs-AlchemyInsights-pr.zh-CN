---
title: 发布敏感度标签
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11015"
- "9000181"
ms.openlocfilehash: 1db4d15b45ff95a643ceca788667de9fb6a8f4bc
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532245"
---
# <a name="how-to-publish-a-sensitivity-label"></a>发布敏感度标签

1. 转到 Microsoft 365 合规中心 > **“信息保护** > **标签策略”**。

1. 选择 **+ 发布标签** 以启动“新”敏感度标签向导。

1. 选择 “**选择要发布的敏感度标签**”。 选择可在应用和服务中可以使用的标签，随后选择“**添加**”。

    **重要**：如果选择子标签，请确保也选择其父标签。

1. 查看所选标签。 若要进行任意更改，请选择" **编辑**;否则，请选择 **下一**。

1. 按照提示配置策略设置。

1. 如果不同的用户或位置需要不同的策略设置，请重复这些步骤。 例如，希望为一组用户创建附加标签，或用户为子集创建不同的默认标签。

1. 如果创建多个可能导致用户或位置发生冲突的标签策略，请查看策略顺序，并根据需要向上或向下移动。 若要更改标签策略的顺序，请选择三个点（更多操作），然后选择“**上移**”或“**下移**”。

完成向导会自动发布标签策略。