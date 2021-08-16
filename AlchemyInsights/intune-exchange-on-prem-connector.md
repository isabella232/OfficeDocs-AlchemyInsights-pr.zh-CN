---
title: Intune Exchange本地连接器
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013954"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange本地连接器

有关在 Intune 和本地托管的 Exchange 之间设置连接器的详细信息，请参阅以下文档：

[在 Azure 中设置 Intune 本地Exchange连接器Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**常见问题：**

问：在尝试设置 Exchange Exchange 连接器时，看到"不支持 Exchange 连接器版本"等错误。 原因可能是什么？

答：你使用的帐户已适当许可 - 它必须具有活动的 Intune 许可证

问：是否可能有多个Exchange连接器？

答：每个组织只能Exchange每个 Intune 租户设置一Exchange连接器。 连接器只能安装在多服务器交换组织的一台服务器上。

此外，不能同时为本地Exchange配置连接器，Exchange Online租户中配置连接器。

问：连接器能否使用 CAS 阵列作为与 Exchange 的连接？

答：指定 CAS 阵列在连接器设置中不受支持。 应仅指定一台服务器，并且应在连接器配置文件（可在 其中找到）中对服务器进行硬编码

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

找到以下条目 ```<ExchangeWebServiceURL />``` ，将 URL 替换为 exchange 服务器。

**示例：**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

有关其他疑难解答，请参阅以下文档[：Intune 本地Exchange疑难解答](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**为连接器启用详细Exchange日志记录**

1. 打开 Exchange 连接器跟踪配置文件进行编辑。  
该文件位于 ：%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**示例：**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. 使用下列键查找 TraceSourceLine：OnPremisesExchangeConnectorService  
  
3. 将 SourceLevel 节点值从 Information ActivityTracing (默认) Verbose ActivityTracing  

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
4. 重新启动 Microsoft Intune Exchange Service  
5. 在 Intune 门户中完全同步，直到它完成，然后将 XML 更改回"信息活动跟踪"并重新启动 Microsoft Intune Exchange 服务。  
6. 日志的位置为 ： `%ProgramData%\Microsoft\Windows Intune Exchange Connector`