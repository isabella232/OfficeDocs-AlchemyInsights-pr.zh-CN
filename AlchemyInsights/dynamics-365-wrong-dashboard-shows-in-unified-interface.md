---
title: Dynamics 365-在 Dynamics 365 统一接口中显示错误的仪表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528541"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 统一接口中显示错误的仪表板

您可能会看到与您所期望的仪表板不同的仪表板的几个原因:

## <a name="the-user-has-set-a-user-default-dashboard"></a>用户已设置用户默认仪表板 

通常, 如果 "**设置为默认**值" 按钮未显示在仪表板命令栏中, 则可以标识用户默认仪表板。 用户默认仪表板将覆盖所有其他默认仪表板, 即使用户的默认仪表板不在当前应用中也是如此。

使用以下解决方法取消设置其默认仪表板。

1. 创建新的个人仪表板。

2. 将该新仪表板设置为用户默认的仪表板。

3. 删除该仪表板。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>在站点地图中设置仪表板

您可能已通过选择仪表板并在 "自定义系统" 下选择 "设置为默认值" 来设置组织的默认仪表板。 但是, 如果用户有权访问, 则在站点地图设计器中定义的仪表板将优先于此仪表板。

若要让用户看到您已设置为组织默认值的仪表板, 您可以执行以下操作之一:

* 在站点地图中设置该仪表板

* 删除对那些用户的站点地图定义的仪表板的访问权限
