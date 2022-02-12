---
title: 'Microsoft Teams: Häufige Probleme bei Kunden in Bildungseinrichtungen'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 9239ca0854b9169ef2e221743ed3b27c00f6e9b0
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62631498"
---
# <a name="teams-common-issues-for-education-customers"></a>Microsoft Teams: Häufige Probleme bei Kunden in Bildungseinrichtungen

**Für Kunden der Microsoft Teams for Education-Version:**

Wenn Sie Hilfe bei der Bereitstellung von Teams zur Unterstützung von Fernunterricht benötigen, besuchen Sie das [FastTrack Center](https://www.microsoft.com/fasttrack), um eine Anfrage zu senden. Hier finden Sie Informationen zu häufig auftretenden Problemen für Microsoft Teams for Education-Kunden:

- Sie sehen sie die Meldung "**Sie verpassen etwas!**" Stellen Sie sicher, dass Sie [Microsoft Teams für Ihre Schule aktivieren](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Bei EDU-Mandanten ist Microsoft Teams standardmäßig nicht aktiviert. Sie müssen es zuerst aktivieren.

- **Neu bei Microsoft Teams?** Lesen Sie [Fernstudium (Lehren und Lernen) in Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4), um die aktuellste Anleitung zur Organisation Ihrer Bildungseinrichtung, zur Unterrichtsplanung, zu virtuellen Besprechungen und zum Teilen von Inhalten mit den Schülern zu erhalten.

- Sobald es aktiviert ist, können Ihre Benutzer Teams ausführen, indem Sie es entweder den [Desktop](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) und [mobile Clients](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) oder über den Browser unter https://teams.microsoft.com installieren.

- **Aktivieren des Teams-Gastzugriffs:** Gehen Sie die [Checkliste für den Teams-Gastzugriff](https://docs.microsoft.com/microsoftteams/guest-access-checklist) durch, und stellen Sie sicher, dass alle Schritte durchgeführt wurden.
    - [Grundlegendes zum Gastzugriff in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Setup – Checkliste für den Microsoft Teams-Gastzugriff](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Beitritt eines Gasts zu einem Team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-Besprechungen und Einwählen**: Benötigen Sie Hilfe beim Aktivieren oder Einrichten von Audiokonferenzen in Microsoft Teams? Wurde dieser Benutzer kürzlich erstellt? Wenn dies der Fall ist, müssen Sie 2 bis 24 Stunden warten, bis die Einstellungen wirksam werden. So überprüfen Sie, ob der Benutzer für Audiokonferenzen lizenziert ist und über eine gebührenpflichtige Standardnummer verfügt:
    1. Wechseln Sie zu "Aktive Benutzer", und wählen Sie den betreffenden Benutzer aus.
    2. Je nach Admin Center-Version müssen Sie entweder **Lizenzen und Apps** auswählen oder unter **Produktlizenzen** auf **Bearbeiten** klicken.
    3. Vergewissern Sie sich, dass für den Benutzer Lizenzen für Audiokonferenzen, Microsoft Teams und Skype for Business Online (Plan 2) ausgewählt sind.
    4. Klicken Sie im Admin Center für Benutzer auf **Alle anzeigen** und dann auf **Teams**.
    5. Klicken Sie im Microsoft Teams Admin Center auf **Altes Portal**.
    6. Klicken Sie im Skype for Business Admin Center auf **Audiokonferenzen** und dann auf **Benutzer**.
    7. Wählen Sie den betreffenden Nutzer aus, und vergewissern Sie sich, dass er über eine gebührenpflichtige Standardnummer verfügt.

    Weitere Informationen finden Sie unter [Microsoft Teams-Anrufpläne](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365). Sie können sich auch an das Microsoft Commerce-Abrechnungsteam wenden, um Fragen zur Lizenzierung zu beantworten.

    Weitere Ressourcen

    - [Besprechungen und Konferenzen in Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audiokonferenz](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Besprechungsrichtlinien**: Besprechungsrichtlinien werden verwendet, um die Features zu steuern, die Besprechungsteilnehmern für Besprechungen, die von Benutzern in Ihrer Organisation geplant werden, zur Verfügung stehen. Nachdem Sie eine Richtlinie erstellt und die gewünschten Änderungen vorgenommen haben, können Sie der Richtlinie Benutzer zuweisen.

    - **Ändern oder Erstellen einer Besprechungsrichtlinie**: Wenn Sie eine Besprechungsrichtlinie ändern oder erstellen möchten, wechseln Sie zum **Microsoft Teams Admin Center > Besprechungen Besprechungsrichtlinien**. Wählen Sie in der Liste eine Richtlinie aus, oder klicken Sie auf **Hinzufügen**. Wenn Sie eine neue Richtlinie erstellen, fügen Sie einen Namen und eine Beschreibung hinzu. Der Name darf keine Sonderzeichen enthalten und nicht mehr als 64 Zeichen lang sein. Wählen Sie die gewünschten Einstellungen aus, und klicken Sie dann auf **Speichern**. 
    
        Nehmen wir beispielsweise an, Sie haben eine Gruppe von Benutzern, und Sie möchten die Bandbreite begrenzen, die für Ihre Besprechung erforderlich ist. Sie erstellen dann eine neue benutzerdefinierte Richtlinie namens „begrenzte Bandbreite“ und deaktivieren die folgenden Einstellungen:

        Unter **Audio & Video**:
        - Deaktivieren Sie **Cloudaufnahme zulassen**.
        - Deaktivieren Sie **IP-Video zulassen**.

        Unter **Inhaltsfreigabe**:

        - Deaktivieren Sie den Bildschirmübertragungsmodus.
        - Deaktivieren Sie **Whiteboard zulassen**.
        - Deaktivieren Sie **Freigegebene Notizen zulassen**.

        **Weisen Sie dann die Richtlinie den Benutzern zu**:

    1. Wechseln Sie in der linken Navigation des Microsoft Teams Admin Centers zu **Benutzer**, und klicken Sie dann den gewünschten Benutzer an.
    2. Wählen Sie den Benutzer aus, indem Sie links neben den Benutzernamen klicken, und klicken Sie dann auf **Einstellungen bearbeiten**.
    3. Wählen Sie unter **Besprechungsrichtlinie** die Richtlinie aus, die Sie zuweisen möchten, und klicken Sie dann auf **Übernehmen**.

    Informationen dazu, wie Sie eine Richtlinie mehreren Benutzern gleichzeitig zuweisen können, finden Sie unter [Batchbearbeitung von Benutzereinstellungen eines Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Oder Sie können Folgendes tun:
    1. Wechseln Sie in der linken Navigation von Microsoft Teams Admin Center zu **Besprechungen > Besprechungsrichtlinien**.
    2. Wählen Sie die gewünschte Richtlinie aus, indem Sie links neben die Richtlinienbezeichnung klicken.
    3. Klicken Sie auf **Benutzer verwalten**.
    4. Suchen Sie im Bereich **Benutzer verwalten** anhand des Anzeigenamens oder des Benutzernamens nach dem Benutzer, wählen Sie den Namen und dann **Hinzufügen** aus. Wiederholen Sie diesen Schritt für jeden Nutzer, den Sie hinzufügen möchten.
    5. Wenn Sie mit dem Hinzufügen von Benutzern fertig sind, klicken Sie auf **Speichern**.

- **Problembehandlung bei fehlender Wähltastatur**:
    - Stellen Sie sicher, dass dem Benutzer eine [Teams-Lizenz](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) zugewiesen wurde.
    - Stellen Sie sicher, dass dem Benutzer ein [Anrufplan](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) zugewiesen wurde.
    - Aktivieren Sie die Benutzer für [Enterprise-VoIP](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Problembehandlung bei Teams-Anmeldung:** Stellen Sie zuerst sicher, dass der [Microsoft Teams-Dienst fehlerfrei funktioniert](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Überprüfen Sie dann, ob häufige Fehlercodes vorhanden sind, und lesen Sie [Warum habe ich Probleme beim Anmelden bei Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Möglicherweise müssen Sie auch [Identitätsmodelle und Authentifizierung in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication) überprüfen.
