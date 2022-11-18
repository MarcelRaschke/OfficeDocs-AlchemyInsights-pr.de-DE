---
title: Aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung können keine E-Mails an/von Office 365 gesendet/empfangen werden.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 1ca1834b5b12c56c4da98efefea9e3569a55e2eb
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66287608"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung können keine E-Mails an/von Office 365 gesendet/empfangen werden.

Wie vom Nachrichtencenter nach MC229914 bestätigt, wurde die Einstellung von TLS 1.0 und TLS 1.1 für Exchange Online E-Mail-Flussendpunkte erzwungen. Bald akzeptiert Office 365 keine TLS 1.0- und TLS 1.1-E-Mail-Verbindungen von externen Quellen mehr. Außerdem verwenden Exchange Online nieMALS TLS 1.0 oder 1.1 zum Senden ausgehender E-Mails. Wenn Probleme aufgrund der TLS 1.0- oder 1.1-Deaktivierung auftreten, tritt möglicherweise einer der folgenden Fehler auf:

- Der Absender erhält NDR zurückgesprungen - "421 4.4.2 Verbindung aufgrund von SocketError abgebrochen"
- Fehler im Warteschleifen-Viewer des lokalen Servers, der E-Mails an Officer 365 sendet: "421 4.4.2-Verbindung wurde aufgrund von SocketError abgebrochen"
- Fehler im Protokoll "Connector senden["](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) auf dem Server, der E-Mails an Office 365 sendet– TLS-Aushandlung mit Fehler SocketError fehlgeschlagen
- Fehler im Protokoll des Sende- oder Empfangsconnectors – "451 5.7.3 Muss zuerst einen STARTTLS-Befehl ausgeben"

Wenn einer der oben genannten Fehler auftritt, stellen Sie sicher, dass auf dem Server, der E-Mails sendet oder empfängt, TLS 1.2 aktiviert ist, indem Sie die folgenden Registrierungsschlüssel überprüfen:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Wenn Sie Änderungen an den oben genannten Registrierungsschlüsseln vornehmen, um TLS 1.2 zu aktivieren, starten Sie den Server neu, damit die Änderungen wirksam werden. Stellen Sie außerdem sicher, dass die neuesten Windows- und Exchange-Updates installiert sind.

Weitere Informationen finden Sie unter:

- [Exchange Server TLS-Anleitung, Teil 1: Vorbereiten für TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-Anleitung Teil 2: Aktivieren von TLS 1.2 und Identifizieren von Clients, die es nicht verwenden – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Grundlegendes zu E-Mail-Szenarien, wenn TLS-Versionen nicht mit Exchange Online vereinbart werden können – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
