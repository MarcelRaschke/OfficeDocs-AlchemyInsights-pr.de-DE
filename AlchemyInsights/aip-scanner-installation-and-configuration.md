---
title: 'AIP-Scanner: Installation und Konfiguration'
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
- "9002278"
- "5119"
ms.openlocfilehash: 10d8b8206cde1d7130b9c5fa0b4134976b1ac1f6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62659254"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-Scanner: Installation und Konfiguration

**Folgen Sie zum Installieren des AIP-Scanners den empfohlenen Richtlinien**:

1. Wenn Sie ein Upgrade und nicht eine Neuinstallation durchführen, folgen Sie den Richtlinien für die [Aktualisierung des Azure Information Protection-Scanners](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) und für den Client für einheitliche Bezeichnungen (siehe [Upgrade des Azure Information Protection-Scanners](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)).
2. Vergewissern Sie sich, dass Sie alle [Anforderungen für Firewall- und Netzwerkinfrastruktur-Einstellungen](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure) erfüllen.
3. Stellen Sie sicher, dass Ihre [Richtlinien](https://docs.microsoft.com/azure/information-protection/configure-policy) auf das automatische Bezeichnen festgelegt sind oder in der jeweiligen Richtlinie eine Standardbezeichnung angegeben ist.
4. Stellen Sie sicher, dass der relevante Dateityp für Bezeichnung/Schutz wie in [Vom Azure Information Protection-Client unterstützte Dateitypen](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) beschrieben konfiguriert ist. Wenn Sie das Standardverhalten ändern möchten, befolgen Sie die Angaben unter [Ändern der Standardschutzebene von Dateien](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Vergewissern Sie sich, dass das für die Ausführung des Scanner-Diensts konfigurierte Benutzerkonto über Berechtigungen für den Zugriff auf alle konfigurierten Repositories verfügt.
6. Wenn weiterhin Probleme auftreten, exportieren Sie die Scanner-Protokolle, und fügen Sie sie Ihrem Supportticket hinzu.

**Protokolle des Azure Information Protection-Scanners exportieren**

1. Navigieren Sie unterhalb des Benutzerkontexts, in dem der Scannerdienst ausgeführt wird, zu %localappdata%\Microsoft\MSIP.
2. Komprimieren Sie alle Inhalte im Ordner "MSIP".
3. Speichern Sie die Protokolle an einem beliebigen Ort, und fügen Sie sie an Ihre Serviceanfrage an.
4. Sie können auch [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps&preserve-view=true) verwenden.

**Weitere Informationen finden Sie unter**:
- [Bereitstellen des Azure Information Protection-Scanners zum automatischen Klassifizieren und Schützen von Dateien](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angeben und Verwenden des Token-Parameters für Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Ausführen eines Suchzyklus und Anzeigen von Berichten für den Scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Nachschlagen in der Azure Information Protection-Dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Anforderungen für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection Client herunterladen](https://www.microsoft.com/download/details.aspx?id=53018)
