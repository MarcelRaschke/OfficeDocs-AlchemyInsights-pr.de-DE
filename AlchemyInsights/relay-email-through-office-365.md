---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3000003"
- "154"
ms.openlocfilehash: c9fb59420acfebcad53db5e8e51ac5bee5a5eb33
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66318783"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails

Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Wenn Sie ein Gerät oder eine Anwendung haben, das/die seit Kurzem nicht mehr funktioniert, sind die häufigsten Probleme:

- **Fehler im Zusammenhang mit der Authentifizierung bei Verwendung der SMTP AUTH-Clientübermittlung**: Weitere Informationen zur Behebung von Problemen finden Sie unter [Fehler: Authentifizierung fehlgeschlagen](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Wir akzeptieren nur TLS 1.2 für sichere Verbindungen mit Microsoft**: Wenn Sie eine sichere Verbindung (TLS) verwenden, stellen Sie sicher, dass Ihr Anwendungsgerät TLS 1.2 unterstützt. Weitere Informationen finden Sie unter [Vorbereiten für TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).

Weitere Probleme und Lösungen finden Sie unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mithilfe von Microsoft 365 oder Office 365 senden](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Um betroffene Geräte anzuzeigen, wechseln Sie zum **Bericht über SMTP AUTH-Clients** im Exchange Admin Center (EAC) unter <https://admin.exchange.microsoft.com/#/reports/smtpauthmailflowdetails>.

**Hinweis**: Exchange Online unterstützt keine Massensendungsszenarien. Um kommerzielle Massen-E-Mails (z. B. Kunden-Newsletter) zu versenden, sollten Sie Drittanbieter verwenden, die auf diese Dienste spezialisiert sind.
