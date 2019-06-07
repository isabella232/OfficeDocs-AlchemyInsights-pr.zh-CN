---
title: 902 (由于重复的对象而产生的同步错误)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757985"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="638d7-102">由于复制对象导致的同步错误</span><span class="sxs-lookup"><span data-stu-id="638d7-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="638d7-103">目录同步完成时, 您可能会收到以下错误消息之一:</span><span class="sxs-lookup"><span data-stu-id="638d7-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="638d7-104">无法更新 Microsoft Online Services 中的此对象, 因为与此对象相关联的以下属性的值可能已与本地目录中的另一个对象相关联。</span><span class="sxs-lookup"><span data-stu-id="638d7-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="638d7-105">您的 Microsoft Online Services 目录中已存在具有相同代理地址的同步对象。</span><span class="sxs-lookup"><span data-stu-id="638d7-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="638d7-106">无法更新此对象, 因为与此对象相关联的以下属性的值可能已经与本地目录服务中的另一个对象相关联: UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="638d7-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="638d7-107">若要确定并解决问题, 请下载并运行[IdFix DirSync 错误修正工具](https://www.microsoft.com/download/details.aspx?id=36832)。</span><span class="sxs-lookup"><span data-stu-id="638d7-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="638d7-108">有关详细信息, 请参阅[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。</span><span class="sxs-lookup"><span data-stu-id="638d7-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
