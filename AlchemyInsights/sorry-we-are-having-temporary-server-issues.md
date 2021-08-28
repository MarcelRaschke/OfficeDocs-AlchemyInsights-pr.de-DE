---
title: Beheben Microsoft 365 Apps Leider wird eine Meldung zu temporären Serverproblemen angezeigt.
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021595"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Beheben der Microsoft 365-Apps mit der Meldung "Leider treten temporäre Serverprobleme auf"

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Internetzugriff auf Microsoft 365 Apps nicht blockieren. Siehe [URLs und IP-Adressbereiche.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Wechseln **Sie** zu  >  **Startausführung,** und geben Sie dann **"services.msc"** ein. Stellen Sie sicher, dass die folgenden Dienste ausgeführt werden:
    - Automatische Einrichtung netzwerkverbundener Geräte
    - Netzwerklistendienst
    - Netzwerkstandortinformationen
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht ausgeführt wird, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc /scannow**

Starten Sie nach Abschluss dieses Befehls den Computer neu.

Ausführliche Informationen finden Sie unter ["Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es später erneut" beim Aktivieren.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)