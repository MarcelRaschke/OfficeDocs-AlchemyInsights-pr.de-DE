---
title: Anmelden bei Windows 10 ohne Kennwort
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 5c604dbd2577df078fc84171caa5f4540ad5b1e2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66417478"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Anmelden bei Windows 10 ohne Kennwort

Um zu vermeiden, dass Sie beim Windows-Start ein Kennwort eingeben müssen, empfehlen wir, eine der Windows Hello sicheren Anmeldeoptionen zu verwenden, z. B. eine PIN, Gesichtserkennung oder Fingerabdruck, falls verfügbar. Wenn Sie die sichere Anmeldung wirklich deaktivieren möchten, lesen Sie unten die Anweisungen "Automatisch bei Windows 10 anmelden".

**Sichern Windows Hello Alternativen zum Kontokennwort**

Wechseln **Sie zu Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Die verfügbaren Anmeldeoptionen werden aufgelistet. Beispiel:

![Anmeldeoptionen.](media/sign-in-options.png)

Klicken oder tippen Sie auf eine der Optionen, um sie zu konfigurieren. Wenn Sie Windows das nächste Mal starten oder entsperren, können Sie die neue Option anstelle eines Kennworts verwenden. 

**Automatische Anmeldung bei Windows 10**

**Hinweis**: Die automatische Anmeldung ist praktisch, führt jedoch zu einem Sicherheitsrisiko, insbesondere, wenn auf Ihren PC mehrere Personen zugreifen können. 

1. Klicken oder tippen Sie auf der Taskleiste auf die Schaltfläche " **Start** ".

2. Geben Sie **netplwiz ein** , und drücken Sie die EINGABETASTE, um das Fenster "Benutzerkonten" zu öffnen.

3. Klicken Sie in **"Benutzerkonten**" auf das Konto, bei dem Sie sich beim Start von Windows automatisch anmelden möchten.

4. Deaktivieren Sie das Kontrollkästchen "Benutzer müssen einen Benutzernamen und ein Kennwort eingeben, um diesen Computer verwenden zu können".

    ![Benutzer müssen eine Option für Benutzername und Kennwort eingeben.](media/users-must-enter-username.png)

5. Klicken Sie auf **OK**. Sie werden aufgefordert, das Kennwort für das ausgewählte Konto einzugeben und zu bestätigen. Klicken Sie zum Abschließen auf **OK**. Wenn Windows 10 das nächste Mal gestartet wird, wird es sich automatisch bei dem von Ihnen ausgewählten Konto anmelden.
