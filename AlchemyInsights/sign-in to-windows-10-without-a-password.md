---
title: Anmelden bei Windows 10 ohne Kennwort
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 5e86865f1acf2628c5557b099e1b093fb51ce72a
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62727297"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Anmelden bei Windows 10 ohne Kennwort

Um zu vermeiden, dass Sie bei Windows Start ein Kennwort eingeben müssen, empfehlen wir, eine der Windows Hello sicheren Anmeldeoptionen wie PIN, Gesichtserkennung oder Fingerabdruck zu verwenden, falls verfügbar. Wenn Sie die sichere Anmeldung wirklich deaktivieren möchten, lesen Sie die Anweisungen unter "Automatische Anmeldung bei Windows 10".

**Sichern Windows Hello Alternativen zum Kontokennwort**

Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Verfügbare Anmeldeoptionen werden aufgelistet. Zum Beispiel: 

![Anmeldeoptionen.](media/sign-in-options.png)

Klicken oder tippen Sie auf eine der Optionen, um sie zu konfigurieren. Wenn Sie Windows das nächste Mal starten oder entsperren, können Sie die neue Option anstelle eines Kennworts verwenden. 

**Automatische Anmeldung bei Windows 10**

**Hinweis**: Die automatische Anmeldung ist praktisch, führt jedoch zu einem Sicherheitsrisiko, insbesondere, wenn auf Ihren PC mehrere Personen zugegriffen werden kann. 

1. Klicken oder tippen Sie auf der Taskleiste auf die Schaltfläche " **Start** ".

2. Geben Sie **"netplwiz"** ein, und drücken Sie die EINGABETASTE, um das Fenster "Benutzerkonten" zu öffnen.

3. Klicken Sie in **Benutzerkonten** auf das Konto, bei dem Sie sich automatisch anmelden möchten, wenn Windows gestartet wird.

4. Deaktivieren Sie das Kontrollkästchen "Benutzer müssen einen Benutzernamen und ein Kennwort eingeben, um diesen Computer verwenden zu können".

    ![Benutzer müssen eine Benutzernamen- und Kennwortoption eingeben.](media/users-must-enter-username.png)

5. Klicken Sie auf **OK**. Sie werden aufgefordert, das Kennwort für das von Ihnen ausgewählte Konto einzugeben und zu bestätigen. Klicken Sie zum Abschließen auf **OK**. Wenn Windows 10 das nächste Mal gestartet wird, wird automatisch das von Ihnen ausgewählte Konto angemeldet.
