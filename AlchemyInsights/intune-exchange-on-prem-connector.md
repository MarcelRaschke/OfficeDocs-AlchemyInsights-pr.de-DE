---
title: Intune Exchange lokalen Connector
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
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013963"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokalen Connector

Ausführliche Informationen zum Einrichten des Connectors zwischen Intune und Exchange, der lokal gehostet wird, finden Sie in der folgenden Dokumentation:

[Einrichten des lokalen Intune-Exchange-Connectors in Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Häufig gestellte Fragen:**

F: Beim Versuch, den Exchange Connector einzurichten, wird ein Fehler angezeigt, z. B. "Die Exchange Connectorversion wird nicht unterstützt". Was könnte die Ursache sein?

A: Das konto, das Sie verwenden, ist entsprechend lizenziert – es muss über eine aktive Intune-Lizenz verfügen.

F: Ist es möglich, mehrere Exchange Connectors zu verwenden?

Antwort: Sie können nur einen Exchange Connector pro Intune-Mandant pro Exchange Organisation einrichten. Der Connector kann nur auf einem Server in einer Exchange-Organisation mit mehreren Servern installiert werden.

Außerdem können Connectors nicht sowohl für Exchange lokalen als auch für Exchange Online im selben Mandanten konfiguriert sein.

F: Kann der Connector ein CAS-Array als Verbindung mit Exchange verwenden?

A: Die Angabe eines CAS-Arrays wird beim Connector-Setup nicht unterstützt. Es sollte nur ein einzelner Server angegeben und in der Connectorkonfigurationsdatei hartcodiert werden, die in

programm data\microsoft\microsoft Intune on premises Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Suchen Sie den folgenden ```<ExchangeWebServiceURL />``` Eintrag, und ersetzen Sie die URL durch den Exchange-Server.

**Beispiel:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Weitere Informationen zur Problembehandlung finden Sie in der folgenden Dokumentation: [Problembehandlung beim lokalen Intune-Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivieren der ausführlichen Protokollierung für den Exchange Connector**

1. Öffnen Sie die Konfigurationsdatei Exchange Connector-Ablaufverfolgung zur Bearbeitung.  
Die Datei befindet sich unter : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Beispiel:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Suchen Sie traceSourceLine mit dem folgenden Schlüssel: OnPremisesExchangeConnectorService  
  
3. Ändern des SourceLevel-Knotenwerts von Information ActivityTracing (Standard) in "Verbose ActivityTracing"  

**Beispiel:**
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
4. Starten Sie den Microsoft Intune Exchange-Dienst neu.  
5. Vollständige Synchronisierung im Intune-Portal, bis es abgeschlossen ist, und ändern Sie dann den XML-Code wieder in "Information ActivityTracing", und starten Sie den Microsoft Intune Exchange-Dienst neu.  
6. Der Speicherort der Protokolle lautet: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`