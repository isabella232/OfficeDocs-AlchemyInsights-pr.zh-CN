---
title: 更新 DNS 记录以便利用当前的托管提供商继续托管网站
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423713"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="715ec-102">更新 DNS 记录以便利用当前的托管提供商继续托管网站</span><span class="sxs-lookup"><span data-stu-id="715ec-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="715ec-103">在" [域](https://portal.office.com/adminportal/home#/Domains) "页面上的域列表中，选择要用于你的网站的域，然后在管理窗格中选择" **DNS 设置** "。</span><span class="sxs-lookup"><span data-stu-id="715ec-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="715ec-104">选择" **+ 新增自定义记录** "，然后输入以下信息：</span><span class="sxs-lookup"><span data-stu-id="715ec-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="715ec-105">对于" **DNS 类型** "，请输入： **A (地址)**</span><span class="sxs-lookup"><span data-stu-id="715ec-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="715ec-106">对于" **主机名或别名** "，请键入： **@**</span><span class="sxs-lookup"><span data-stu-id="715ec-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="715ec-107">对于" **IP 地址** "，请键入网站当前托管位置的静态 IP 地址（例如 172.16.140.1）。</span><span class="sxs-lookup"><span data-stu-id="715ec-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="715ec-p101">必须是该网站的 *静态*  IP 地址，不能是  *动态*  IP 地址。 请与您的网站的托管网站核实，确保可以获得您的公共网站的静态 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="715ec-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="715ec-110">选择" **保存** "。</span><span class="sxs-lookup"><span data-stu-id="715ec-110">Select **Save**.</span></span> 
    
<span data-ttu-id="715ec-111">此外，您可以创建 CNAME 记录以帮助客户找到您的网站。</span><span class="sxs-lookup"><span data-stu-id="715ec-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="715ec-112">选择" **+ 新增自定义记录** "，然后输入以下信息：</span><span class="sxs-lookup"><span data-stu-id="715ec-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="715ec-113">对于" **DNS 类型** "，请输入： **CNAME (别名)**</span><span class="sxs-lookup"><span data-stu-id="715ec-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="715ec-114">对于" **主机名或别名** "，请键入： **www**</span><span class="sxs-lookup"><span data-stu-id="715ec-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="715ec-115">对于" **指向地址** "，请键入网站的完全限定域名 (FQDN)，例如 contoso.com。</span><span class="sxs-lookup"><span data-stu-id="715ec-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="715ec-116">选择“保存”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="715ec-116">Select **Save**.</span></span> 
    

