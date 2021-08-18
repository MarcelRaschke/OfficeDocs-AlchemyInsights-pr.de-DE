---
title: Aktivieren des Kennwortrückschreibens in Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118203"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivieren des Kennwortrückschreibens in Azure AD Connect

Wenn Sie das Rückschreiben für die Self-Service-Kennwortzurücksetzung aktivieren möchten, aktivieren Sie zuerst die Rückschreibeoption in Azure AD Connect. Führen Sie auf Ihrem Azure AD Connect-Server die folgenden Schritte aus:

1. Melden Sie sich bei Ihrem Azure AD Connect-Server an, und starten Sie den Konfigurations-Assistenten **Azure AD Connect**.
2. Klicken Sie auf der **Begrüßungsseite** auf **Konfigurieren**.
3. Wählen Sie auf dem Seite **Weitere Aufgaben** die Option **Synchronisierungsoptionen anpassen** aus, und klicken Sie dann auf **Weiter**.
4. Geben Sie auf der Seite **Mit Azure AD verbinden** die Anmeldeinformationen für Ihren Azure-Mandanten ein, und klicken Sie dann auf **Weiter**.
5. Klicken sie auf den Filterseiten **Verzeichnisse verbinden** und **Domänen-/OE** auf **Weiter**.
6. Wählen Sie auf der Seite **Optionale Funktionen** das Kästchen neben **Kennwortrückschreiben** aus, und klicken Sie dann auf **Weiter**.
7. Klicken Sie auf der Seite **Bereit zum Konfigurieren** auf **Konfigurieren** und warten Sie, bis der Vorgang abgeschlossen ist.
8. Wenn die Option zum Abschließen der Konfiguration angezeigt wird, klicken Sie auf **Beenden**.

Wenn das Kennwortrückschreiben in Azure AD Connect aktiviert ist, konfigurieren Sie Azure AD SSPR für das Rückschreiben.  Führen Sie die folgenden Schritte aus, um das Kennwortrückschreiben in SSPR zu aktivieren:

1. Melden Sie sich mit einem globalen Administratorkonto beim Azure-Portal an.
2. Suchen Sie nach **Azure Active Directory**, wählen Sie es aus, klicken Sie auf **Kennwortzurücksetzung** und dann auf **Lokale Integration**.
3. Legen Sie die Option für **Kennwörter in Ihr lokales Verzeichnis zurückschreiben?** auf **Ja** fest.
4. Legen Sie die Option für **Zulassen, dass Benutzer Konten entsperren können, ohne das Kennwort zurückzusetzen?** auf **Ja** fest.
5. Klicken Sie abschließend auf **Speichern**.

Weitere Informationen finden Sie unter [Aktivieren des Zurückschreibens einer Azure Active Directory Self-Service-Kennwortzurücksetzung in eine lokale Umgebung](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Wenn ein Administrator das Kennwort eines Benutzers im Azure-Portal zurücksetzt, dann wird das Kennwort in das lokale System zurückgeschrieben, wenn dieser Benutzer ein Verbundbenutzer ist oder mit einem Kennworthash synchronisiert wird. Dies Funktionalität benötigt eine Azure Premium-Lizenz (P1 oder P2) und ist zurzeit im Office-Administratorportal nicht unterstützt.
