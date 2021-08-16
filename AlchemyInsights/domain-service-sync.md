---
title: 域服务同步
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057848"
---
# <a name="domain-service-synchronization"></a>域服务同步

Azure Active Directory 域服务 (Azure AD DS) 托管域中的对象和凭据可以在域中本地创建，也可以从 Azure Active Directory (Azure AD) 租户进行同步。 首次部署 Azure AD DS 时，将配置并启动自动单向同步以从 Azure AD 复制对象。 此单向同步将继续在后台运行，使 Azure AD DS 托管域保持最新状态，并更新来自 Azure AD 的任何更改。 Azure AD DS 不会同步回 Azure AD。

有关域服务Azure Active Directory的详细信息，请参阅[域服务同步](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)。 
