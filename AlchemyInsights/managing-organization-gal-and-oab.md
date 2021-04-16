---
title: 管理组织全局地址列表和脱机通讯簿
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794822"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>管理组织全局地址列表 (GAL) 和脱机通讯簿 (OAB)

全局地址列表 (GAL) 是组织中已启用邮件的对象（可接收电子邮件的任何类型的收件人）的列表。 每个组织中会自动创建一个 GAL。 可按组织或位置创建其他 GAL 来分隔用户，但一个用户一次只能查看和使用一个 GAL。

有些电子邮件客户端（例如 Outlook for Windows）会下载 GAL，以便脱机使用。 这称为脱机通讯簿 (OAB)。 在 Exchange Online 中，OAB 每 8 个小时仅更新一次，然后客户端必须下载它以更新本地 OAB 副本。 任何收件人更改首先必须在 GAL 中可见，之后再显示在 OAB 中。

下面是一些常用的 GAL 和 OAB 程序：

- 出于多种原因，你可能希望在 GAL 中隐藏某些对象。 请参阅[在地址列表中隐藏收件人](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)。
- 如果需要向特定用户组提供组织的 GAL 的自定义视图，请参阅 [Exchange Online中的通讯簿策略](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)。
- [在 Exchange Online 中创建全局地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)，要了解如何使用 GAL 权限，请参阅 [Exchange Online 中的地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)。 请注意，如果你创建了新的 GAL，可能还需要创建一个新的 OAB。 请参阅[脱机通讯簿程序](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)。
