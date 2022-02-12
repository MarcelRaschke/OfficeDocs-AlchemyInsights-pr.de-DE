---
title: Konfigurieren Sie den Dienstverbindungspunkts (SCP).
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 598fb2f5e036b3d482db37dc5271c05e4d3de2b2
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62687191"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurieren Sie den Dienstverbindungspunkt (SCP).

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Grund**: Das SCP-Objekt kann nicht gelesen und die Azure AD-Mandanteninformationen können nicht abgerufen werden
- **Lösung**: Weitere Informationen finden Sie im Abschnitt [Konfigurieren eines Dienstverbindungspunkts](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Aktionsplan**

- Überprüfen Sie, ob das Gerät das Gruppenrichtlinienobjekt für die kontrollierte Prüfung erhalten hat.
- Stellen Sie sicher, dass das Gruppenrichtlinienobjekt die Registrierungsschlüssel erstellt hat.
- Stellen Sie sicher, dass Sie 2 Schlüssel mit Ihrer Verzeichnis-ID und Ihrer Onmicrosoft-Domäne erstellt haben.

**Konfigurieren der clientseitigen Registrierungseinstellung für SCP**

Verwenden Sie das folgende Beispiel, um ein Gruppenrichtlinienobjekt (Group Policy Object, GPO) zu erstellen, um eine Registrierungseinstellung bereitzustellen, mit der ein SCP-Eintrag in der Registrierung Ihrer Geräte konfiguriert wird.

1. Öffnen Sie eine Gruppenrichtlinien-Verwaltungskonsole und erstellen Sie ein neues Gruppenrichtlinienobjekt in Ihrer Domäne.
     - Geben Sie Ihrem neu erstellten Gruppenrichtlinienobjekt einen Namen (z. B. ClientSideSCP).

2. Bearbeiten Sie das Gruppenrichtlinienobjekt und suchen Sie den folgenden Pfad: **Computerkonfiguration > Einstellungen > Windows-Einstellungen > Registrierung**.

3. Klicken Sie mit der rechten Maustaste auf **Registrierung** und wählen Sie **Neu > Registrierungselement**.

4. Auf der Registerkarte **Allgemein** konfigurieren Sie Folgendes:
  
- **Aktion**: Aktualisieren
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Schlüsselpfad**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Wertname**: TenantId
    
- **Werttyp**: REG_SZ
    
- **Wertdaten**: Die GUID oder Verzeichnis-ID Ihrer Azure AD-Instanz (Dieser Wert befindet sich unter **Azure-Portal > Azure Active Directory > Eigenschaften > Verzeichnis-ID**)
 
- Klicken Sie auf **OK**.
 
5. Klicken Sie mit der rechten Maustaste auf **Registrierung** und wählen Sie **Neu > Registrierungselement**.

6. Auf der Registerkarte **Allgemein** konfigurieren Sie Folgendes:
  
- **Aktion**: Aktualisieren
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Schlüsselpfad**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Wertname**: TenantName
    
- **Werttyp**: REG_SZ
    
- **Wertdaten**: Ihr verifizierter Domänenname, wenn Sie eine Verbundumgebung wie AD FS verwenden. Ihr verifizierter Domainname oder Ihr Domainname onmicrosoft.com (z. B. contoso.onmicrosoft).com, wenn Sie eine verwaltete Umgebung verwenden

- Klicken Sie auf **OK**.

7. Schließen Sie den Editor für das neu erstellte Gruppenrichtlinienobjekt.

8. Verknüpfen Sie das neu erstellte Gruppenrichtlinienobjekt mit der gewünschten Organisationseinheit, die domänenverbundene Computer enthält, die zu Ihrer kontrollierten Rollout-Population gehören.

Weitere Informationen finden Sie unter [Kontrollierte Prüfung des hybriden Azure AD-Joins – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) und  [Fehlerbehebung für hybride Azure Active Directory-Geräte | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









