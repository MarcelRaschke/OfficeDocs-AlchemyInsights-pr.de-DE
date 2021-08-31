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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744594"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Beheben der Microsoft 365-Apps mit der Meldung "Wir können zur zeit keine Verbindung herstellen"

Hinweis: Wenn Sie eine ältere Version von Windows verwenden (z. B. Windows 7 SP1, Windows Server 2008 R2), verwenden Sie die [einfache Korrektur,](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) um TLS 1.2 standardmäßig zu aktivieren. Weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

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

Ausführliche Informationen finden Sie unter ["Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es später erneut" beim Aktivieren Office aus Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).