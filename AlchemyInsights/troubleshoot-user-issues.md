---
title: Behandeln von Problemen im Zusammenhang mit Benutzern
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: c63e92cfb802685f622535fe4c098780ad7e9c68
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65723252"
---
# <a name="announcements"></a>Ankündigungen

Folgen Sie den Anweisungen von Google zum Testen der Kompatibilität, um zu testen, ob Ihre Apps betroffen sind. Die Anleitung von Google finden Sie hier: https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.

Verwenden Sie die Systemwebansicht oder den Systembrowser, wenn Sie Ihre Benutzer mit Google-Privatanwenderkonten anmelden. Weitere Informationen finden Sie unter [Probleme bei der Anmeldung bei Anwendungen (nur Chrome-Browser)](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Ich kann keinen neuen Benutzer in meinem Azure AD-Verzeichnis erstellen**

Führen Sie die folgenden Schritte aus, wenn keine neuen Benutzer in Azure AD erstellt werden können:

1. Vergewissern Sie sich, dass Sie berechtigt sind, einen neuen Standardbenutzer zu erstellen. Nur wer über die Rolle eines globalen Administrators oder Benutzeradministrators in Azure Active Directory (AD) verfügt, kann einen neuen Standardbenutzer erstellen. Wenn Sie keine dieser Rollen besitzen, bitten Sie einen Administrator, Sie einer dieser Rollen hinzuzufügen oder das neue Benutzerkonto für Sie zu erstellen.
2. Stellen Sie sicher, dass der Benutzername zu der Domäne gehört, die in Azure AD verifiziert wurde. Wenn es in Azure AD keine verifizierten benutzerdefinierten Domänennamen gibt, können Sie Ihre anfängliche Azure AD-Domäne verwenden, welche mit "*.onmicrosoft.com" endet.
3. Stellen Sie sicher, dass der Benutzername zu einer Domäne gehört, die nicht mit Azure AD über Ihr lokales AD verbunden ist. Benutzer mit über lokale Umgebungen verbundenen Domänennamen können nicht in der Cloud hinzugefügt werden.
4. Stellen Sie sicher, dass noch kein anderer Benutzer oder Kontakt den Benutzernamen aufweist, den Sie dem neuen Benutzer zuweisen möchten. Benutzernamen müssen in Azure AD eindeutig sein.
5. Weitere Informationen für Ihr Azure AD finden Sie unter [Azure AD-Rollen und -Administratoren](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators).
6. Informieren Sie sich über die [Domänennamen,](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) für Ihr Azure AD.
7. Überprüfen Sie die [Überwachungsprotokolle](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit), um detailliertere Informationen zu einem kürzlich erstellten oder gelöschten Benutzer zu erhalten, z. B. wer die Aktion ausgeführt hat und wann.
8. Weitere Informationen zum Hinzufügen neuer Benutzer finden Sie unter [Verwenden des Azure-Portals zum Erstellen eines neuen Benutzers in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Weitere Informationen zu Administratorrollenberechtigungen in Azure AD finden Sie unter [Administratorrollen für Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Details zum Erstellen eines Benutzers mithilfe von Azure AD PowerShell finden Sie unter [Azure AD PowerShell zum Erstellen eines neuen Benutzers](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Probleme bei der Self-Service-Registrierung**

Führen Sie die folgenden Schritte aus, um Probleme im Zusammenhang mit der Self-Service-Registrierung zu behandeln:

1. Um die Self-Service-Registrierung mit Ihren Anwendungen zu verwenden, aktivieren Sie zuerst die Self-Service-Registrierung für Ihren Mandanten. 
2. Wenn Sie eine Anwendung für die Unterstützung der Self-Service-Registrierung aktivieren möchten, fügen Sie sie Ihrem Benutzerablauf hinzu. Wenn Sie das nächste Mal zur Anmeldeseite für diese Anwendung wechseln, wird die folgende Option angezeigt: ***Noch kein Konto? Erstellen Sie eines!***. Dadurch wird der Self-Service-Registrierungsvorgang gestartet.
3. Informationen zum Verwenden der Self-Service-Registrierung für das Ausfüllen einer Organisation in Azure AD finden Sie unter [Self-Service-Registrierung für Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Nachdem Sie den Benutzerablauf einer oder mehreren Anwendungen zugeordnet haben, können sich Benutzer, die diese App besuchen, mithilfe der im Benutzerablauf konfigurierten Optionen registrieren und ein Gastkonto erhalten. Weitere Informationen zum Registrieren und Erhalten eines Gastkontos finden die Benutzer unter [Self-Service-Registrierung für Gastbenutzer](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

**Probleme beim Einladen externer Benutzer**

Führen Sie den folgenden Schritt aus, um Probleme beim Einladen eines externen Benutzers zu behandeln:

Stellen Sie sicher, dass Sie die Einladung eines Benutzers an die E-Mail-Adresse senden, die dem Namen entspricht, mit dem sich der Benutzer anmeldet. Wenn Sie die Einladung an die Proxy-E-Mail-Adresse eines Benutzers senden, kann der Benutzer sie nicht nutzen. Weitere Informationen finden Sie in der [Dokumentation zu Azure Active Directory B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Ich kann einem Benutzer keine Lizenzen zuweisen**

Führen Sie die folgenden Schritte aus, um Probleme im Zusammenhang mit dem Zuweisen von Lizenzen an Benutzer zu behandeln:

1. Stellen Sie sicher, dass Sie zum Verwalten von Benutzerlizenzen ein Konto mit einer der dazu erforderlichen Administratorrollen verwenden: globaler Administrator, Lizenzadministrator oder Benutzeradministrator. Sie können die Rolle des Benutzers auf der Registerkarte **Verzeichnisrolle** auf dem Benutzerblatt überprüfen.
2. Wenn Sie gerade das Azure-Portal verwenden und die Lizenzzuweisung fehlschlägt, klicken Sie auf die Benachrichtigung in der oberen rechten Ecke. Damit wird ein Bereich mit Details zu dem Fehler geöffnet. In den meisten Fällen reicht dies aus, um das Problem zu verstehen und es beheben zu können.
3. Bevor einem Benutzer eine Lizenz zugewiesen werden kann, muss die Eigenschaft **Verwendungsort** für den Benutzer festgelegt werden. Vergewissern Sie sich, dass diese Eigenschaft für den Benutzer festgelegt wurde, indem Sie die Registerkarte **Profil** im "Benutzer"-Bereich überprüfen.
4. Vergewissern Sie sich, dass ausreichend Lizenzen für das Produkt verfügbar sind, das Sie zuweisen möchten. Sie können die Anzahl der verfügbaren Lizenzen im Azure-Portal unter [Azure Active Directory -> Lizenzen -> Alle Produkte](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products) einsehen.
5. Möglicherweise verfügt der Benutzer bereits über eine andere Lizenz, deren Dienste mit denen in der neuen Lizenz in Konflikt stehen, die Sie zuweisen möchten. Wenn der Benutzer beispielsweise den Dienst Exchange Online (Plan 1) aktiviert hat, können Sie keine Lizenz mit Exchange Online (Plan 2) zuweisen. Deaktivieren Sie einen der Dienste, um die neue Lizenzzuweisung zu ermöglichen. Falls Sie das Azure-Portal oder PowerShell-Cmdlets verwenden, werden auf der Seite zu den **Problemdetails** die Dienste aufgeführt, die den Konflikt verursachen.
6. Wenn das Entfernen einer Lizenz fehlschlägt, verfügt der Benutzer möglicherweise über weitere Lizenzen mit Diensten, die von den Diensten abhängen, die Sie entfernen möchten. Falls Sie das Azure-Portal oder PowerShell-Cmdlets verwenden, werden in der Fehlermeldung die Dienste aufgeführt, die Abhängigkeiten aufweisen.
7. Wenn Sie verstehen möchten, warum eine Lizenz für einen Benutzer hinzugefügt/entfernt wurde (beispielsweise, wer sonst noch in Ihrer Organisation Änderungen vorgenommen hat), überprüfen Sie die Überwachungsprotokolle. Legen Sie den Filter auf **Lizenzaktivitäten** fest, um alle Änderungen, einschließlich derjenigen Person, die sie vorgenommen hat, anzeigen zu lassen.
8. Falls Sie Exchange Online verwenden, wurden einige Benutzer in Ihrem Mandanten möglicherweise nicht ordnungsgemäß mit demselben Proxyadresswert konfiguriert. In solchen Fällen werden möglicherweise allgemeine Fehlermeldungen angezeigt, wenn ein Lizenzvorgang fehlschlägt. [Dieser Artikel](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) enthält weitere Informationen zu diesem Problem, einschließlich Informationen zum Herstellen einer [Verbindung mit Exchange Online mithilfe von Remote-PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Führen Sie dieses Exchange Online-Cmdlet aus, um zu ermitteln, welche Benutzer in Ihrem Mandanten dieselbe Proxyadresse enthalten:

Ausführen

`Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses`
