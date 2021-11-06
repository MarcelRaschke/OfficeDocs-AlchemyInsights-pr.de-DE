---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 7897661204ca6bce5c2ac2450a153c222809c6ab
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799146"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails

Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Wenn Sie ein Gerät oder eine Anwendung haben, das/die seit Kurzem nicht mehr funktioniert, sind die häufigsten Probleme:

- **Fehler im Zusammenhang mit der Authentifizierung bei Verwendung der SMTP AUTH-Clientübermittlung**: Weitere Informationen zur Behebung von Problemen finden Sie unter [Fehler: Authentifizierung fehlgeschlagen](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Wir akzeptieren nur TLS 1.2 für sichere Verbindungen mit Microsoft**: Wenn Sie eine sichere Verbindung (TLS) verwenden, stellen Sie sicher, dass Ihr Anwendungsgerät TLS 1.2 unterstützt. Weitere Informationen finden Sie unter [Vorbereiten für TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).

Weitere Probleme und Lösungen finden Sie unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mithilfe von Microsoft 365 oder Office 365 senden](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Um betroffene Geräte anzuzeigen, wechseln Sie zum **Bericht über SMTP AUTH-Clients** im Exchange Admin Center (EAC) unter <https://admin.exchange.microsoft.com/#/reports/smtpauthmailflowdetails>.

**Hinweis**: Exchange Online unterstützt keine Massensendungsszenarien. Um kommerzielle Massen-E-Mails (z. B. Kunden-Newsletter) zu versenden, sollten Sie Drittanbieter verwenden, die auf diese Dienste spezialisiert sind.
