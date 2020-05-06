---
title: 管理组织全局地址列表和脱机通讯簿
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022388"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="8dddd-102">管理组织全局地址列表 (GAL) 和脱机通讯簿 (OAB)</span><span class="sxs-lookup"><span data-stu-id="8dddd-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="8dddd-103">全局地址列表 (GAL) 是组织中已启用邮件的对象（可接收电子邮件的任何类型的收件人）的列表。</span><span class="sxs-lookup"><span data-stu-id="8dddd-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="8dddd-104">每个组织中会自动创建一个 GAL。</span><span class="sxs-lookup"><span data-stu-id="8dddd-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="8dddd-105">可按组织或位置创建其他 GAL 来分隔用户，但一个用户一次只能查看和使用一个 GAL。</span><span class="sxs-lookup"><span data-stu-id="8dddd-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="8dddd-106">有些电子邮件客户端（例如 Outlook for Windows）会下载 GAL，以便脱机使用。</span><span class="sxs-lookup"><span data-stu-id="8dddd-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="8dddd-107">这称为脱机通讯簿 (OAB)。</span><span class="sxs-lookup"><span data-stu-id="8dddd-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="8dddd-108">在 Exchange Online 中，OAB 每 8 个小时仅更新一次，然后客户端必须下载它以更新本地 OAB 副本。</span><span class="sxs-lookup"><span data-stu-id="8dddd-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="8dddd-109">任何收件人更改首先必须在 GAL 中可见，之后再显示在 OAB 中。</span><span class="sxs-lookup"><span data-stu-id="8dddd-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="8dddd-110">下面是一些常用的 GAL 和 OAB 程序：</span><span class="sxs-lookup"><span data-stu-id="8dddd-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="8dddd-111">出于多种原因，你可能希望在 GAL 中隐藏某些对象。</span><span class="sxs-lookup"><span data-stu-id="8dddd-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="8dddd-112">请参阅[在地址列表中隐藏收件人](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)。</span><span class="sxs-lookup"><span data-stu-id="8dddd-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="8dddd-113">如果需要向特定用户组提供组织的 GAL 的自定义视图，请参阅 [Exchange Online中的通讯簿策略](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)。</span><span class="sxs-lookup"><span data-stu-id="8dddd-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="8dddd-114">[在 Exchange Online 中创建全局地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)，要了解如何使用 GAL 权限，请参阅 [Exchange Online 中的地址列表](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)。</span><span class="sxs-lookup"><span data-stu-id="8dddd-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="8dddd-115">请注意，如果你创建了新的 GAL，可能还需要创建一个新的 OAB。</span><span class="sxs-lookup"><span data-stu-id="8dddd-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="8dddd-116">请参阅[脱机通讯簿程序](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)。</span><span class="sxs-lookup"><span data-stu-id="8dddd-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
