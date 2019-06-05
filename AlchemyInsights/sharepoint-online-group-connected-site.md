---
title: 将组添加到 SharePoint 网站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719472"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>在 SharePoint Online 中创建组连接的网站

<p><strong>创建或重新创建组连接的网站时遇到了几个常见的问题。&nbsp;</strong></p>  <p>1.如果已删除某个组及其连接的网站, 并且想要创建另一个具有相同 URL 的网站, 则需要永久删除以前的网站。</p>  <ul>  <li>下载<a title="SPO 命令行管理程序" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO 命令行</a> -管理程序有关如何开始使用 powershell 的详细信息<a title=", 请参阅 SharePoint Online 命令行管理程序入门" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">SharePoint Online 命令行</a>管理程序入门。 <br /><br /></li>  <li>使用<a title="Remove-spodeletedsite 从已删除的网站中删除网站" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-spodeletedsite</a> powershell cmdlet。</li>  </ul>  <p>如果要创建组连接的网站并收到警告<strong>"另一个具有相同别名的组已存在"</strong>, 请从管理中心检查<a title="Office 365 中的现有组。" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">来自管理中心的 Office 365</a>。 若要解决此问题, 请删除现有组 (如果不再需要它) 或创建具有分配了不同别名的网站。&nbsp;</p>  <p><strong>可以使用不同的方法来创建和使用 SharePoint 的新式组。&nbsp;</strong></p>  <ol>  <li>您可以将现有网站连接到 Office 365 组。 有关详细信息, 请<a title="参阅 Connect a Office 365 group Using the SharePoint user ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">使用 SharePoint 用户 ineterface</a>连接 Office 365 组。</li>  <li>若要创建 Office 365 组连接的网站, 需要创建团队网站。 有关详细信息, 请<a title="参阅在 SharePoint 中创建团队网站" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">在 SharePoint 中创建团队网站。</a></li>  </ol>

