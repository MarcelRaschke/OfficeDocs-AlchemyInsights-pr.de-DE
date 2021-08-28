---
title: Aktivierungsproblem– Wir können derzeit keine Verbindung herstellen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998151"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Beheben der Microsoft 365-Apps "Wir können derzeit keine Verbindung herstellen"

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Internetzugriff auf Microsoft 365 Apps nicht blockieren. Siehe [Microsoft-URLs und IP-Adressbereiche.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Wechseln **Sie** zu  >  **Startausführung,** und geben Sie dann **"services.msc"** ein. Stellen Sie sicher, dass die folgenden Dienste ausgeführt werden:
    - Automatische Einrichtung netzwerkverbundener Geräte
    - Netzwerklistendienst
    - Netzwerkstandortinformationen
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht ausgeführt wird, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc /scannow**

Starten Sie nach Abschluss dieses Befehls den Computer neu.

Ausführliche Informationen finden Sie unter ["Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es später erneut", wenn Sie Office aus Microsoft 365 aktivieren.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)