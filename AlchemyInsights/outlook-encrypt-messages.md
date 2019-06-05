---
title: Web 上的 Outlook 中的 S/MIME
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/1/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 16454927730d49ba1ec64380145b0fde1294850b
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34720207"
---
# <a name="encrypt-email-messages-in-outlook"></a>在 Outlook 中加密电子邮件

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Office 365 邮件加密是基于 Microsoft Azure 权限管理 (Azure RMS) 构建的, 这是 Azure 信息保护的一部分。如果你的订阅包括 Azure 权限管理或 Azure 信息保护,<strong style="mso-bidi-font-weight: normal;">则无需执行任何操作来手动启用或激活</strong>权限管理服务。</span></p> <p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">根据客户反馈, 我们将不再启用 Exchange 邮件流规则, 以在默认情况下, 在租户中自动对包含特定类型敏感信息的出站电子邮件进行加密。&nbsp;相反, 我们将提供有关如何进行此操作的详细说明。&nbsp;有关如何创建传输规则以加密敏感信息的其他详细信息, 请参阅<a href="https://aka.ms/OmeEtr">本文</a>。</span><u></u><span style="text-decoration: line-through;"></span></p> <ul> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: Symbol; mso-fareast-font-family: Symbol; mso-bidi-font-family: Symbol;"><span style="mso-list: Ignore;">&nbsp;如果&nbsp;Web 上的 Outlook (以前称为 OWA): 撰写电子邮件时, 只需在 OWA 中单击 "保护" 即可。 &nbsp; &nbsp; </span> </span> <span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"> <strong style="mso-bidi-font-weight: normal;"></strong> <strong></strong>默认情况下&lsquo;, 这将应用 "&rsquo;不转发" 权限。单击 "<strong>更改权限</strong>", 然后选择 "<strong>加密</strong>" 仅加密邮件。</span></li> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;如果使用<strong style="mso-bidi-font-weight: normal;">outlook 客户端</strong>: 从 outlook 2013 或2016发送加密邮件, 或 outlook 2016 for Mac, 请选择 " &agrave;选项权限", 然后选择所需的保护选项。 &nbsp; &nbsp;</span></li> <li style="text-indent: -.25in; mso-list: l0 level1 lfo1;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;&nbsp;若要自动对发送给特定收件人或外部合作伙伴组织的<strong style="mso-bidi-font-weight: normal;">所有电子邮件进行加密</strong>, 需要在 Exchange 管理中心中创建邮件流传输规则。本<span style="color: black;"><a href="https://docs.microsoft.com/en-us/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities">支持文章</a></span>中提供了详细说明</span></li> </ul>

