---
title: 配置预配服务
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480744"
---
# <a name="configuring-the-provision-service"></a>配置预配服务

若要使自动用户预配正常工作，Azure AD 需要允许其连接到 Workday Web 服务 API 的有效凭据。 此外，Workday 到 AD 用户预配应用的"测试连接"按钮还会验证它能否连接到与 AD 域关联的 Azure AD Connect 预配代理。

如果 Azure 门户在保存凭据时返回错误，请按照下面的建议步骤操作：

1. 确认你已配置 Workday 集成系统用户帐户，如教程部分所述在 [Workday 中配置集成系统用户](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。
2. 使用服务管理控制台确认 Azure AD Connect 预配代理服务已在本地 Windows 服务器上启动并运行。 还可以单击"查看本地代理"按钮，在 Azure 门户中检查代理的状态。
3. 确保使用"工作日用户名"字段的格式输入username@workday-tenant-name。 如果缺少 workday-tenant-name，则 Workday 身份验证将失败。
4. 如果要配置与 Workday 实现租户的集成，请注意 Workday 租户的计划停机时间。 工作日已安排其实施租户在周末的停机时间 (通常从星期五晚上到星期六上午) 并且此停机时间窗口中的连接故障是一个已知问题，一旦实现租户重新联机，就会自动解决该问题。
5. 在极少数情况下，如果集成系统用户的密码因租户刷新而更改，或者帐户已锁定或已过期，则也可能看到此错误。 Please check the status of the Integration System user with your Workday administrator.

有关为自动预配配置工作日的更多详细信息，请参阅教程：为自动用户预配配置[Workday。](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
