---
title: Intune Exchange 本地连接器
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791368"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="4bf78-102">Intune Exchange 本地连接器</span><span class="sxs-lookup"><span data-stu-id="4bf78-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="4bf78-103">有关在本地托管的 Intune 和 Exchange 之间设置连接器的详细信息，请参阅以下文档：</span><span class="sxs-lookup"><span data-stu-id="4bf78-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="4bf78-104">在 Microsoft Intune Azure 中设置 Intune 本地 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="4bf78-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="4bf78-105">**常见问题：**</span><span class="sxs-lookup"><span data-stu-id="4bf78-105">**FAQ:**</span></span>

<span data-ttu-id="4bf78-106">问：当试图设置 Exchange 连接器时，看到一个错误，如 "不支持 Exchange Connector 版本"。</span><span class="sxs-lookup"><span data-stu-id="4bf78-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="4bf78-107">原因可能是什么？</span><span class="sxs-lookup"><span data-stu-id="4bf78-107">What could be the cause?</span></span>

<span data-ttu-id="4bf78-108">A：你使用的帐户已得到正确许可-必须拥有活动的 Intune 许可证</span><span class="sxs-lookup"><span data-stu-id="4bf78-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="4bf78-109">问：是否可以有多个 Exchange 连接器？</span><span class="sxs-lookup"><span data-stu-id="4bf78-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="4bf78-110">A：只能针对每个 Exchange 组织设置一个每个 Intune 租户的 Exchange connector。</span><span class="sxs-lookup"><span data-stu-id="4bf78-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="4bf78-111">连接器仅可安装在多服务器 exchange 组织中的一台服务器上。</span><span class="sxs-lookup"><span data-stu-id="4bf78-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="4bf78-112">此外，不能为在同一个租户中配置的 Exchange 内部部署和 Exchange Online 配置连接器。</span><span class="sxs-lookup"><span data-stu-id="4bf78-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="4bf78-113">问：连接器是否可以使用 CAS 阵列作为与 Exchange 的连接？</span><span class="sxs-lookup"><span data-stu-id="4bf78-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="4bf78-114">A：连接器安装程序中指定的 CAS 阵列不是受支持的配置。</span><span class="sxs-lookup"><span data-stu-id="4bf78-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="4bf78-115">应仅指定一台服务器，并且应将其硬编码在连接器配置文件中，该文件可在中找到</span><span class="sxs-lookup"><span data-stu-id="4bf78-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="4bf78-116">program data\microsoft\microsoft Intune on 本地 Exchange 连接器 \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="4bf78-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="4bf78-117">找到以下条目 ```<ExchangeWebServiceURL />``` 并将 URL 替换为 exchange 服务器。</span><span class="sxs-lookup"><span data-stu-id="4bf78-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="4bf78-118">**示例**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="4bf78-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="4bf78-119">请参阅以下文档以获取其他故障排除：对 [Intune 本地 Exchange 连接器进行故障排除](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="4bf78-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="4bf78-120">**为 Exchange connector 启用详细日志记录**</span><span class="sxs-lookup"><span data-stu-id="4bf78-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="4bf78-121">打开 Exchange Connector 跟踪配置文件以进行编辑。</span><span class="sxs-lookup"><span data-stu-id="4bf78-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="4bf78-122">文件位于：%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="4bf78-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="4bf78-123">**示例**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="4bf78-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="4bf78-124">使用以下项查找 TraceSourceLine： OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="4bf78-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="4bf78-125">将默认)  (的信息 ActivityTracing 中的 SourceLevel 节点值更改为 Verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="4bf78-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="4bf78-126">**示例：**</span><span class="sxs-lookup"><span data-stu-id="4bf78-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="4bf78-127">重新启动 Microsoft Intune Exchange 服务</span><span class="sxs-lookup"><span data-stu-id="4bf78-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="4bf78-128">在 Intune 门户中进行完全同步，直到它完成，然后将 XML 更改回 "信息 ActivityTracing" 并重新启动 Microsoft Intune Exchange 服务。</span><span class="sxs-lookup"><span data-stu-id="4bf78-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="4bf78-129">日志的位置是： `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="4bf78-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>