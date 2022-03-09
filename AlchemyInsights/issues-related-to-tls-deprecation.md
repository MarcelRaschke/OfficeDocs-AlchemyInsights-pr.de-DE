---
title: E-Mails können aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung nicht an/von Office 365 gesendet/empfangen werden.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 0657673e901f73fbbe76c651f9b9324bf6beb376
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63246293"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>E-Mails können aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung nicht an/von Office 365 gesendet/empfangen werden.

Wie vom Nachrichtencenter nach MC229914 bestätigt, wurde die Deaktivierung von TLS 1.0 und TLS 1.1 für Exchange Online Nachrichtenflussendpunkte erzwungen. Bald akzeptieren Office 365 keine TLS 1.0- und TLS 1.1-E-Mail-Verbindungen von externen Quellen mehr. Außerdem verwenden Exchange Online niemals TLS 1.0 oder 1.1, um ausgehende E-Mails zu senden. Wenn Aufgrund der TLS 1.0- oder 1.1-Deaktivierung Probleme auftreten, tritt möglicherweise einer der folgenden Fehler auf:

- Absender erhält NDR-Bounceback - '421 4.4.2 Connection dropped due to SocketError'
- Fehler in der Warteschlangenanzeige des lokalen Servers, der E-Mails an Officer 365 sendet- '421 4.4.2 Verbindung aufgrund von SocketError verworfen'
- Fehler im Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError
- Fehler im Protokollprotokoll zum Senden oder Empfangen von Connectors – "451 5.7.3 Muss zuerst einen STARTTLS-Befehl ausgeben"

Wenn die oben genannten Fehler auftreten, stellen Sie sicher, dass auf dem Server, der E-Mails sendet oder empfängt, TLS 1.2 aktiviert ist, indem Sie die folgenden Registrierungsschlüssel überprüfen:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Wenn Sie änderungen an den obigen Registrierungsschlüsseln vornehmen, um TLS 1.2 zu aktivieren, starten Sie den Server neu, damit die Änderungen wirksam werden. Stellen Sie außerdem sicher, dass die neuesten Windows und Exchange Updates installiert sind.

Weitere Informationen finden Sie unter:

- [Exchange Server TLS-Leitfaden, Teil 1: Vorbereiten auf TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-Leitfaden Teil 2: Aktivieren von TLS 1.2 und Identifizieren von Clients, die es nicht verwenden – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Grundlegendes zu E-Mail-Szenarien, wenn tls-Versionen nicht mit Exchange Online vereinbart werden können – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
