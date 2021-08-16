---
title: 客户端身份验证故障排除证书部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020794"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>客户端身份验证故障排除证书部署

“Intune NDES/SCEP”和“PKCS/PFX”客户端证书配置文件通常与其他配置文件类型（例如 Wifi、VPN 和电子邮件）结合使用，允许用户对公司资源进行身份验证。 将这些配置文件类型关联到客户端证书配置文件时，依赖于成功部署该配置文件。

初始基础结构设置和客户端证书配置文件的关联配置通常需要进行故障排除。 有关成功设置 NDES 连接器的分步指南和故障排除指南以找出与证书部署相关的问题，请参阅： 

- [配置基础结构以支持使用 Intune 中的 SCEP](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [有关使用 Microsoft Intune 解决 SCEP 证书配置文件问题的概述](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

使用引用的 powershell 脚本来帮助验证配置。 有关详细信息，请参阅 [Intune 证书连接器验证脚本](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)。

  
**其他常见问题**

**尝试在 NDES 连接器服务器上安装 Intune 证书连接器时，收到消息 “无法验证证书申请中的密码，可能已被占用。请通过此请求获取新密码进行提交。”**  

此消息表示你需要以管理员身份运行证书连接器安装文件。

在某些环境中，运行 Intune 证书的服务器必须使用代理服务器连接到 Intune，因此证书连接器必须使用代理。 在某些情况下，NDES 连接器会忽略配置的代理设置，可能需要在 LocalSystem 的安全上下文中运行代理设置的配置。 
 
解决方案是将 Internet Explorer 作为系统运行，并在 IE 中配置代理。 重新启动 Intune 连接器服务后，NDES 连接器将连接到 Intune。

**用户设备无法再从 NDES 接收 SCEP 证书。**

颁发给 NDES 服务器并在 NDES 连接器安装过程中指定的客户端身份验证证书可能已过期或缺失。若要解决此问题，请执行以下操作： 
 
1. 卸载 NDES 连接器。  
2. 使用以上详细信息，请求新客户端身份验证或服务器身份验证证书： 
 
    - 使用者名称：CN=external fqdn  
    - 使用者备选名称（均为必填项）：DNS=external fqdn, DNS=internal fqdn 
 
3. 重新安装带有新证书的 NDES 连接器。