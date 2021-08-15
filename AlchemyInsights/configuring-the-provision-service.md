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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033268"
---
# <a name="configuring-the-provision-service"></a>配置预配服务

若要使自动用户预配正常工作，Azure AD 需要允许其连接到 Workday Web 服务 API 的有效凭据。 此外，Workday 到 AD 用户预配应用的"测试连接"按钮还将验证它能否连接到与 AD 域关联的 Azure AD 连接预配代理。

如果 Azure 门户在保存凭据时返回错误，请按照下面的建议步骤操作：

1. 确认你已配置 Workday 集成系统用户帐户，如教程部分在 Workday 中配置 [集成系统用户所述](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。
2. 使用服务管理连接，确认 Azure AD 连接设置代理服务已在本地 Windows 服务器上运行。 还可以单击"查看本地代理"按钮，在 Azure 门户中检查代理的状态。
3. 确保使用 username@workday-tenant-name 格式输入"Workday Username"字段的值。 如果缺少 workday-tenant-name，则 Workday 身份验证将失败。
4. 如果要配置与 Workday 实现租户的集成，请注意 Workday 租户的计划停机时间。 工作日已安排在周末 (通常从星期五晚上到星期六上午) 的实现租户的停机时间) 在此停机时间窗口期间的连接故障是一个已知问题，一旦实现租户重新联机，就会自动解决。
5. 在极少数情况下，如果集成系统用户的密码由于租户刷新而更改，或者帐户已锁定或已过期，则也可能看到此错误。 Please check the status of the Integration System user with your Workday administrator.

有关配置 workday 以实现自动设置的更多细节，请参阅 [教程：为自动用户设置配置 Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。
