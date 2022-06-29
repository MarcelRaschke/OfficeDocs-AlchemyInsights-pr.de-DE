---
title: Beheben von Gruppenprobleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004358"
- "7814"
ms.date: 01/15/2021
ms.openlocfilehash: 135363f847eb2d0a7be8bcf20b9c8aac5f6dda79
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66371667"
---
# <a name="troubleshoot-group-issues"></a>Beheben von Gruppenprobleme

**Ich muss einer Azure AD-Rolle eine Gruppe zuweisen**

Führen Sie die folgenden Schritte aus, um einer Azure AD-Rolle eine Azure Active Directory-Gruppe (AD) zuzuweisen:

1. Erstellen Sie eine neue Gruppe – Um eine neue Gruppe zu erstellen:

    a. Melden Sie sich im Azure AD-Admin Center mit Berechtigungen für einen Administrator für privilegierte Rollen oder für einen globalen Administrator an. 
    b. Wählen Sie Azure Active Directory > Gruppen > Alle Gruppen > Neue Gruppe aus. 
    c. Erstellen Sie die Gruppe.

2. Weisen Sie der Gruppe die Rolle zu, entweder während der Erstellung der Gruppe oder nachdem die Gruppe erstellt wurde.

    a. Um der Gruppe eine Rolle zum Zeitpunkt der Gruppenerstellung zuzuweisen, aktivieren Sie die Umschaltfläche Azure AD-Rollen können der Gruppe zugewiesen werden und erstellen Sie die Gruppe.
    b. Um der Gruppe eine Rolle zuzuweisen, nachdem sie erstellt wurde, navigieren Sie zur Registerkarte Zugewiesene Rollen für die neu erstellte Gruppe und weisen Sie der Gruppe die Rolle zu.

**Ich muss die Mitgliedschaft in einer Gruppe, der eine Azure AD-Rolle** zugewiesen wurde, verwalten.

1. Um das Erhöhen von Rechten zu verhindern, können standardmäßig nur privilegierte Rollenadministratoren und globale Administratoren die Mitgliedschaft einer Gruppe ändern, die einer Rolle zugewiesen ist. Sie können jedoch auswählen, ob Sie einen Besitzer für eine solche Gruppe auswählen möchten und diese Aufgabe delegieren. Weitere Informationen finden Sie unter [Verwenden von Cloud-Gruppen zum Verwalten von Rollenzuweisungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Allgemeine Fragen und Tipps zur Fehlerbehebung zum Zuweisen von Rollen zu Gruppen in Azure AD finden Sie unter [Fehlerbehebung bei Rollen, die Cloud-Gruppen zugewiesen sind](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dynamische Gruppen**

1. Wenn Sie die integrierten Benutzerattribute nicht finden können, stellen Sie sicher, dass sich das Attribut in der Liste der unterstützten Eigenschaften befindet.
2. Wenn Sie nach integrierten Geräteattributen suchen, stellen Sie sicher, dass sich das Attribut in der Liste der Geräteattribute befindet 
3. Zusätzlich zu den integrierten Benutzer- und Geräteattributen können Sie auch [Erweiterungsattribute](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) verwenden. Nach dem Synchronisieren von Erweiterungsattributen aus lokalem Windows Server AD oder einer verbundenen SaaS-Anwendung sollten die Attribute in der Dropdown-Liste des Regel-Generators angezeigt werden. Der benutzerdefinierte Attributname kann im Verzeichnis gefunden werden, indem das Attribut eines Benutzers mit PowerShell abgefragt und nach dem Attributnamen gesucht wird. Diese können auch beim Erstellen von Regeln in der Regelsyntax verwendet werden.
4. Stellen Sie sicher, dass Ihr Mandant über die entsprechende Lizenz verfügt. Für dynamische Gruppen muss der Mandant über eine Azure AD P1 Premium-Lizenz verfügen. Auf die Liste der Azure AD-Lizenzpläne kann [hier](https://azure.microsoft.com/pricing/details/active-directory/) zugegriffen werden. Auf Lizenzpläne für Enterprise Mobility + Security kann [hier](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing) zugegriffen werden.
5. Stellen Sie sicher, dass der Benutzer, der die dynamische Gruppe erstellt, ein globaler Administrator, ein Intune-Administrator, ein Gruppenadministrator oder ein Benutzeradministrator ist.
6. Bitte geben Sie der Gruppe Zeit, sich zu füllen. Abhängig von der Größe Ihres Mandanten kann es bis zu 24 Stunden dauern, bis die Gruppe zum ersten Mal oder nach einer Regeländerung gefüllt wird.
7. Weitere Informationen finden Sie unter [Erstellen von attributbasierten Regeln für die dynamische Gruppenmitgliedschaft](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Ich muss eine Gruppe löschen**

1. Gruppen können mit dem Cmdlet Remove-AzureADGroup im Azure AD Powershell-Modul aus dem Verzeichnis gelöscht werden.
2. Bevor Sie versuchen, eine synchronisierte Gruppe in Azure AD zu löschen, stellen Sie sicher, dass Sie alle zugewiesenen Lizenzen gelöscht haben, um Fehler zu vermeiden.
3. Weitere Informationen zum Löschen von Gruppen finden Sie unter [Löschen einer Gruppe mit einer zugewiesenen Lizenz](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Ich muss eine gelöschte Gruppe wiederherstellen**

1. Wenn eine Office 365-Gruppe gelöscht wird, kann sie nur bis zu 30 Tage vor dem dauerhaften Löschen wiederhergestellt werden. Nach dem dauerhaften Löschen kann die Gruppe nicht mehr wiederhergestellt werden. Weitere Informationen zum Wiederherstellen von Gruppen finden Sie [hier](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Diese Funktionalität wird für Sicherheitsgruppen und Verteilergruppen nicht unterstützt.
3. Stellen Sie sicher, dass Sie berechtigt sind, eine Office 365-Gruppe wiederherzustellen. Globale Administratoren, Gruppenadministratoren, Benutzerkontoadministratoren, Intune-Dienstadministratoren, Partner-Tier1- oder -Tier2-Support und der Besitzer der Gruppe können eine Gruppe wiederherstellen.
4. Wenn eine dynamische Gruppe gelöscht und wiederhergestellt wird, wird sie als neue Gruppe betrachtet und gemäß der Regel erneut aufgefüllt. Dieser Vorgang kann bis zu 24 Stunden dauern.
5. Weitere Informationen zum Wiederherstellen einer gelöschten Gruppe finden Sie unter [Wiederherstellen einer gelöschten Office 365-Gruppe in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfiguration der Gruppenablaufrichtlinie**

1. Diese Funktionalität wird nur für Office 365-Gruppen unterstützt, nicht jedoch für Sicherheitsgruppen und Verteilergruppen.
2. Für die Konfiguration und Verwendung der Ablaufrichtlinie für Office 365-Gruppen ist eine Azure AD Premium-Lizenz erforderlich.
3. Derzeit kann nur eine Ablaufrichtlinie für Office 365-Gruppen auf einem Mandanten konfiguriert werden.
4. Nur globale Administratoren, Gruppenadministratoren, Benutzeradministratoren und der Eigentümer der Gruppe können eine Gruppe erneuern.
5. Wenn eine Office 365-Gruppe abgelaufen ist, wird sie gelöscht und kann nur bis zu 30 Tage vor dem dauerhaften Löschen wiederhergestellt werden. Nach dem dauerhaften Löschen kann die Gruppe nicht mehr wiederhergestellt werden. Weitere Informationen zum Wiederherstellen von Gruppen finden Sie [hier](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Aktivitätsbasierte automatische Verlängerung**

Benutzeraktivitäten von SharePoint, Outlook und Teams können eine automatische Gruppenerneuerung auslösen. Aktivitäten werden 35 Tage vor Ablauf einer Gruppe überprüft. Wenn während des aktuellen Gruppenlebenszyklus Aktivitäten stattfinden, wird die Gruppe automatisch erneuert und es wird keine E-Mail-Benachrichtigung an die Gruppeninhaber gesendet.

**Benachrichtigungszeitpunkt für abgelaufene Gruppen**

1. E-Mail-Benachrichtigungen werden 30 Tage, 15 Tage und 1 Tag vor Ablauf der Gruppe an die Eigentümer der Office 365-Gruppe gesendet.
2. Wenn Sie den Ablauf zum ersten Mal einrichten, werden alle Gruppen, die älter als das Ablaufintervall sind, auf 35 Tage bis zum Ablauf festgelegt.
3. Das Ablaufdatum der Gruppe wird basierend auf dem Erneuerungsdatum der Gruppe berechnet, nicht basierend auf dem Aktualisierungsdatum der Richtlinie. Wenn die Ablaufrichtlinie aktualisiert wird, ändert sich das Ablaufdatum nicht.
4. Weitere Informationen finden Sie unter [Richtlinie zum Ablauf von Gruppen und Verlängerungs-E-Mails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) und [Wiederherstellen einer gelöschten Office 365-Gruppe in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Berechtigung zum Erstellen einer Gruppe**

Stellen Sie sicher, dass Sie berechtigt sind, eine neue Gruppe zu erstellen. Globale Administratoren können die Gruppenerstellung im Microsoft Azure-Portal oder im Access Panel deaktivieren. Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen die entsprechenden Berechtigungen zu erteilen.

1. [Erstellen einer neuen Gruppe und hinzufügen von Mitgliedern im Microsoft Azure-Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Erstellen von Gruppen in Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Deaktivieren der Gruppenerstellung in Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Verwalten, wer in Office 365 Gruppen erstellen kann](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Deaktivieren der Begrüßungsbenachrichtigung für Office 365 über Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD-Verwaltungsrollen](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Verwalten von Gruppenerstellungsberechtigungen**

1. Globale Administratoren können Gruppenerstellungsberechtigungen für Sicherheits- oder Office 365-Gruppen verwalten, die im Azure-Portal oder im Access Panel erstellt wurden, indem **Benutzer Sicherheitsgruppen in Azure-Portalen erstellen** oder **Benutzer Office 365-Gruppen in Azure-Portaleinstellungen** unter **Alle Gruppen > Allgemein (Einstellungen)** erstellen können.
2. Sie können die Gruppenerstellung auch einschränken, um eine Gruppe von Benutzern auszuwählen, wenn Sie über eine Azure AD P1 Premium-Lizenz verfügen.

**Deaktivieren der Begrüßungsbenachrichtigung für neue Mitglieder einer Office 365-Gruppe**

Die Willkommensbenachrichtigung, die an Benutzer gesendet wird, die Office 365-Gruppen hinzugefügt werden, kann deaktiviert werden, indem `UnifiedGroupWelcomeMessageEnabled` in PowerShell auf **False** gesetzt wird. Informationen zu dieser Einstellung finden Sie [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













