---
title: Verwenden von TeamViewer für die Remoteverwaltung von Intune-Geräten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: ca29e2db0690db821f08cac52e22bdfff156bfa4
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63178015"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Verwenden von TeamViewer für die Remoteverwaltung von Intune-Geräten

Von Intune verwaltete Geräte können mithilfe von [TeamViewer](https://www.teamviewer.com/) remote verwaltet werden.

Führen Sie die folgenden Schritte aus, um Intune mithilfe von TeamViewer zu verwalten: 

Beginnen Sie damit, dass Sie Anmeldeinformationen von TeamViewer abrufen, um den TeamViewer-Connector in Intune einzurichten. Auf diese Weise kann der Administrator Anmeldeinformationen in der Benutzeroberfläche des TeamViewer-Connectors unter „Geräte“ eingeben. Hierbei handelt es sich um einen einmaligen Vorgang zum Herstellen der Verknüpfung zwischen Intune und dem TeamViewer-Dienst.

**Teil 1: Starten einer Sitzung mit einem Remotegerät**

1. Wählen Sie unter **Alle Geräte** das Gerät aus, mit dem Sie eine Remotesitzung starten möchten.
2. Wählen Sie unter **...Mehr** die Option **Neue Remoteunterstützungssitzung** aus.
3. Wählen Sie **Ja** aus, um zu bestätigen, dass Sie eine Remotesitzung einrichten möchten.
    Nachdem die Anforderung zur „Initiierung einer neuen Remotesitzung“ vom TeamViewer-Dienst bestätigt wurde, wird unter den Details des Bereichs „Übersicht“ (oder „Essentials“) für das Gerät eine Option **Remotesitzung starten** angezeigt. Wählen Sie **Mehr anzeigen** aus, um den Bereich zu erweitern und den Status der Remoteunterstützung anzuzeigen.
4. Wählen Sie **Remotesitzung starten** aus, um die Sitzung auf der Administratorseite zu initiieren.
5. Wählen Sie das Herunterladen der TeamViewer-Binärdatei (Windows) aus, und wählen Sie **Ausführen** aus.<br/>
    **Hinweis**: Sie können alle Webbrowserseiten ignorieren, die auf der TeamViewer-Website geöffnet sind.

6. Bestätigen Sie die Anforderung der TeamViewer-App zur Vornahme von Änderungen an dem Gerät (nur Windows).
7. Die TeamViewer-App wird gestartet und enthält den Sitzungscode, um die Verbindung mit dem Remotegerät zu authentifizieren.

**Teil 2: Auf dem Gerät, das das Ziel einer Remotesitzung ist**

1. Öffnen Sie das Intune-Unternehmensportal.
2. Suchen Sie nach einer Benachrichtigungskennzeichnung: „Ihr IT-Administrator fordert die Kontrolle über dieses Geräts für eine Remoteunterstützungssitzung an“, und wählen Sie die Benachrichtigung aus.
3. Wählen Sie das Herunterladen der TeamViewer-Anwendung aus, oder bestätigen Sie den Download der TeamViewer-App aus dem App Store, und wählen Sie **Ausführen** aus.
    **Hinweis**: Sie können alle Webbrowserseiten ignorieren, die auf der TeamViewer-Website geöffnet sind.

4. Bestätigen Sie die Anforderung der TeamViewer-App zur Vornahme von Änderungen an dem Gerät (nur Windows).
5. Die TeamViewer-App wird gestartet und enthält den Sitzungscode, um die Verbindung mit dem Remotegerät zu authentifizieren.
6. In einem Popup werden Sie gefragt, ob Sie den Start der Sitzung zulassen möchten.

**Hinweis**: Die vom TeamViewer-Dienst generierten Sitzungscodes können nur einmalig verwendet werden. Wenn die Verbindung getrennt wird, müssen Sie:

1. Die Instanz der TeamViewer-App auf dem Remotegerät und auf der Administratorarbeitsstation schließen.
2. Das Unternehmensportal auf dem Remotegerät schließen.
3. Eine „Neue Remoteunterstützungssitzung“ aus dem Verwaltungsportal initiieren.
4. Das Unternehmensportal auf dem Remotegerät erneut öffnen, um die neue Benachrichtigung zu erhalten.
5. Die TeamViewer-App herunterladen und wie zuvor sowohl auf dem Remotegerät als auch auf der Administratorarbeitsstation öffnen.