---
title: Dynamics 365 - Dynamics 365 统一界面中错误的仪表板显示
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101472"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 统一界面中显示的错误仪表板

你可能会看到不同于预期仪表板的仪表板，原因有多种：

## <a name="the-user-has-set-a-user-default-dashboard"></a>用户已设置用户默认仪表板 

通常，如果仪表板命令栏中未显示"设置为默认值"按钮，则您可以标识用户的默认仪表板。 用户默认仪表板将覆盖所有其他默认仪表板，即使用户的默认仪表板不在当前应用中。

使用以下解决方法取消设置其默认仪表板。

1. 创建新的个人仪表板。

2. 将新仪表板设置为用户默认值。

3. 删除该仪表板。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>在站点地图中设置仪表板

通过选择仪表板并选择"自定义系统"下的"设置为默认值"，你可能已设置组织默认仪表板。 但是，如果用户有权访问此仪表板，则网站地图设计器中定义的仪表板将优先于此仪表板。

若要让用户看到已设置为组织默认设置的仪表板，可以：

* 在站点地图中设置该仪表板

* 删除这些用户对站点地图定义的仪表板的访问权限
