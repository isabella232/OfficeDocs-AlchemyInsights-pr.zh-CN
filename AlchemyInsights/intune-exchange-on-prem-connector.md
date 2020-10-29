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
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange 本地连接器

有关在本地托管的 Intune 和 Exchange 之间设置连接器的详细信息，请参阅以下文档：

[在 Microsoft Intune Azure 中设置 Intune 本地 Exchange 连接器](https://docs.microsoft.com/intune/exchange-connector-install)

**常见问题：**

问：当试图设置 Exchange 连接器时，看到一个错误，如 "不支持 Exchange Connector 版本"。 原因可能是什么？

A：你使用的帐户已得到正确许可-必须拥有活动的 Intune 许可证

问：是否可以有多个 Exchange 连接器？

A：只能针对每个 Exchange 组织设置一个每个 Intune 租户的 Exchange connector。 连接器仅可安装在多服务器 exchange 组织中的一台服务器上。

此外，不能为在同一个租户中配置的 Exchange 内部部署和 Exchange Online 配置连接器。

问：连接器是否可以使用 CAS 阵列作为与 Exchange 的连接？

A：连接器安装程序中指定的 CAS 阵列不是受支持的配置。 应仅指定一台服务器，并且应将其硬编码在连接器配置文件中，该文件可在中找到

program data\microsoft\microsoft Intune on 本地 Exchange 连接器 \ OnpremiseExchangeConnectorServiceConfiguration.xml

找到以下条目 ```<ExchangeWebServiceURL />``` 并将 URL 替换为 exchange 服务器。

**示例**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

请参阅以下文档以获取其他故障排除：对 [Intune 本地 Exchange 连接器进行故障排除](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**为 Exchange connector 启用详细日志记录**

1. 打开 Exchange Connector 跟踪配置文件以进行编辑。  
文件位于：%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**示例**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. 使用以下项查找 TraceSourceLine： OnPremisesExchangeConnectorService  
  
3. 将默认)  (的信息 ActivityTracing 中的 SourceLevel 节点值更改为 Verbose ActivityTracing  

**示例：**
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
4. 重新启动 Microsoft Intune Exchange 服务  
5. 在 Intune 门户中进行完全同步，直到它完成，然后将 XML 更改回 "信息 ActivityTracing" 并重新启动 Microsoft Intune Exchange 服务。  
6. 日志的位置是： `%ProgramData%\Microsoft\Windows Intune Exchange Connector`