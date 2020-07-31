---
title: 客户端身份验证故障排除证书部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509044"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="36739-102">客户端身份验证故障排除证书部署</span><span class="sxs-lookup"><span data-stu-id="36739-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="36739-103">“Intune NDES/SCEP”和“PKCS/PFX”客户端证书配置文件通常与其他配置文件类型（例如 Wifi、VPN 和电子邮件）结合使用，允许用户对公司资源进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="36739-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="36739-104">将这些配置文件类型关联到客户端证书配置文件时，依赖于成功部署该配置文件。</span><span class="sxs-lookup"><span data-stu-id="36739-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="36739-105">初始基础结构设置和客户端证书配置文件的关联配置通常需要进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="36739-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="36739-106">有关成功设置 NDES 连接器的分步指南和故障排除指南以找出与证书部署相关的问题，请参阅：</span><span class="sxs-lookup"><span data-stu-id="36739-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="36739-107">配置基础结构以支持使用 Intune 中的 SCEP</span><span class="sxs-lookup"><span data-stu-id="36739-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="36739-108">有关使用 Microsoft Intune 解决 SCEP 证书配置文件问题的概述</span><span class="sxs-lookup"><span data-stu-id="36739-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="36739-109">使用引用的 powershell 脚本来帮助验证配置。</span><span class="sxs-lookup"><span data-stu-id="36739-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="36739-110">有关详细信息，请参阅 [Intune 证书连接器验证脚本](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)。</span><span class="sxs-lookup"><span data-stu-id="36739-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="36739-111">**其他常见问题**</span><span class="sxs-lookup"><span data-stu-id="36739-111">**Other common issues**</span></span>

<span data-ttu-id="36739-112">**尝试在 NDES 连接器服务器上安装 Intune 证书连接器时，收到消息 “无法验证证书申请中的密码，可能已被占用。请通过此请求获取新密码进行提交。”**</span><span class="sxs-lookup"><span data-stu-id="36739-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="36739-113">此消息表示你需要以管理员身份运行证书连接器安装文件。</span><span class="sxs-lookup"><span data-stu-id="36739-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="36739-114">在某些环境中，运行 Intune 证书的服务器必须使用代理服务器连接到 Intune，因此证书连接器必须使用代理。</span><span class="sxs-lookup"><span data-stu-id="36739-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="36739-115">在某些情况下，NDES 连接器会忽略配置的代理设置，可能需要在 LocalSystem 的安全上下文中运行代理设置的配置。</span><span class="sxs-lookup"><span data-stu-id="36739-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="36739-116">解决方案是将 Internet Explorer 作为系统运行，并在 IE 中配置代理。</span><span class="sxs-lookup"><span data-stu-id="36739-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="36739-117">重新启动 Intune 连接器服务后，NDES 连接器将连接到 Intune。</span><span class="sxs-lookup"><span data-stu-id="36739-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="36739-118">**用户设备无法再从 NDES 接收 SCEP 证书。**</span><span class="sxs-lookup"><span data-stu-id="36739-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="36739-119">在 NDES 连接器安装过程中，颁发给 NDES 服务器和指定的客户端身份验证证书可能已过期或缺失。</span><span class="sxs-lookup"><span data-stu-id="36739-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="36739-120">要解决这一问题，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="36739-120">To resolve:</span></span> 
 
1. <span data-ttu-id="36739-121">卸载 NDES 连接器。</span><span class="sxs-lookup"><span data-stu-id="36739-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="36739-122">使用以上详细信息，请求新客户端身份验证或服务器身份验证证书：</span><span class="sxs-lookup"><span data-stu-id="36739-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="36739-123">使用者名称：CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="36739-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="36739-124">使用者备选名称（均为必填项）：DNS=external fqdn, DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="36739-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="36739-125">重新安装带有新证书的 NDES 连接器。</span><span class="sxs-lookup"><span data-stu-id="36739-125">Reinstall the NDES connector with the new certificate.</span></span>