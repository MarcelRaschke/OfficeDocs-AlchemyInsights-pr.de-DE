---
title: Intune lokalen Exchange-Connector
ms.author: mandia
author: mandia
manager: dougeby
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003775"
- "6732"
ms.date: 04/21/2020
ms.openlocfilehash: 3393f9fe90d7a4e9dc18930473bb1fd60e89cc3e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66258346"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune lokalen Exchange-Connector

Ausführliche Informationen zum Einrichten des Connectors zwischen Intune und Exchange, der lokal gehostet wird, finden Sie in der folgenden Dokumentation:

[Einrichten des Intune lokalen Exchange-Connectors in Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**HÄUFIG GESTELLTE FRAGEN:**

F: Beim Versuch, den Exchange-Connector einzurichten, wird ein Fehler wie "Die Exchange Connector-Version wird nicht unterstützt" angezeigt. Was könnte die Ursache sein?

A: Das Konto, das Sie verwenden, ist entsprechend lizenziert – es muss über eine aktive Intune-Lizenz verfügen.

F: Ist es möglich, mehrere Exchange-Connectors zu haben?

A: Sie können nur einen Exchange-Connector pro Intune Mandanten pro Exchange-Organisation einrichten. Der Connector kann nur auf einem Server in einer Exchange-Organisation mit mehreren Servern installiert werden.

Außerdem können Keine Connectors für lokale Exchange-Konfiguration und Exchange Online im selben Mandanten konfiguriert sein.

F: Kann der Connector ein CAS-Array als Verbindung mit Exchange verwenden?

A: Das Angeben eines CAS-Arrays ist keine unterstützte Konfiguration im Connectorsetup. Es sollte nur ein einzelner Server angegeben und in der Connectorkonfigurationsdatei hartcodiert werden, die in

Programmdaten\microsoft\microsoft Intune lokaler Exchange-Connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Suchen Sie den folgenden Eintrag ```<ExchangeWebServiceURL />``` , und ersetzen Sie die URL durch den Exchange-Server.

**Beispiel:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Weitere Informationen zur Problembehandlung finden Sie in der folgenden Dokumentation: [Problembehandlung beim Intune lokalen Exchange-Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivieren der ausführlichen Protokollierung für den Exchange-Connector**

1. Öffnen Sie die Konfigurationsdatei für die Exchange Connector-Ablaufverfolgung zur Bearbeitung.  
Die Datei befindet sich unter : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Beispiel:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Suchen Sie die TraceSourceLine mit dem folgenden Schlüssel: OnPremisesExchangeConnectorService  
  
3. Ändern des SourceLevel-Knotenwerts von Information ActivityTracing (Standard) in Verbose ActivityTracing  

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
4. Neustarten des Microsoft Intune Exchange-Diensts  
5. Vollständige Synchronisierung in Intune Portal, bis es abgeschlossen ist, und ändern Sie dann den XML-Code wieder in "Information ActivityTracing", und starten Sie den Microsoft Intune Exchange-Dienst neu.  
6. Der Speicherort der Protokolle lautet: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`