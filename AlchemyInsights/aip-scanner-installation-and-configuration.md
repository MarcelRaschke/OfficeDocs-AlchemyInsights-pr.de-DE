---
title: 'AIP-Scanner: Installation und Konfiguration'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: f7f81bc65313d86feb34761b4a9e6f6444607f72
ms.sourcegitcommit: 88adb5a8ce6c6cdcda5b28796aad30c5d13fb02b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/07/2022
ms.locfileid: "67618661"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-Scanner: Installation und Konfiguration

**Folgen Sie zum Installieren des AIP-Scanners den empfohlenen Richtlinien**:

1. Lesen Sie die Anweisungen für eine der folgenden Themen:

    - Upgrades (keine Erstinstallationen) finden Sie unter [Upgrade des Azure Information Protection-Scanners](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).

    - Klassische Clientupgrades finden Sie [unter Upgrade des Azure Information Protection-Scanners](https://docs.microsoft.com/previous-versions/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner).

    - Sehen Sie sich für Standardbereitstellungen das Video ["Installieren des lokalen AIP-Scanners" (7:41)](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/mip-scanner-deployment-watch-our-video/ba-p/2023277?attachment-id=32620) an.

1. Stellen Sie sicher, dass Sie alle Anforderungen an Firewalls und Netzwerkinfrastruktureinstellungen erfüllen. Weitere Informationen finden Sie unter [Firewalls und Netzwerkinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).

1. Richtlinien entsprechend festlegen:

    - Verwenden Sie die automatische Bezeichnung, oder fügen Sie eine Standardbezeichnung in die Richtlinie ein. Weitere Informationen finden Sie unter [Informationen zu Vertraulichkeitsbezeichnungen](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

    - Wenn Sie ein Upgrade des klassischen Clients durchführen, befolgen Sie die Richtlinien unter [Konfigurieren der Azure Information Protection-Richtlinie](https://docs.microsoft.com/previous-versions/azure/information-protection/configure-policy).

1. Bezeichnung/Schutz für relevante Dateitypen konfigurieren:

    - Informationen zu dateitypen, die vom Azure Information Protection Client für einheitliche Bezeichnungen unterstützt werden, finden Sie unter [Unterstützte Dateitypen für Klassifizierung und Schutz](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-file-types#supported-file-types-for-classification-and-protection).

    - Wenn Sie im klassischen Client arbeiten und die Standardschutzebene für Dateien ändern möchten, lesen Sie [die vom Azure Information Protection (AIP)-Client für einheitliche Bezeichnungen unterstützten Dateitypen](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-file-types).

1. Vergewissern Sie sich, dass das für die Ausführung des Scanner-Diensts konfigurierte Benutzerkonto über Berechtigungen für den Zugriff auf alle konfigurierten Repositories verfügt. Weitere Informationen finden Sie unter [Konfigurieren von Superbenutzern für Azure Information Protection- und Discoverydienste oder Datenwiederherstellung](https://docs.microsoft.com/azure/information-protection/configure-super-users).

1. Wenn Sie den Client für einheitliche Bezeichnungen verwenden, beheben Sie häufige Probleme bei der Bereitstellung des [Scanners mithilfe von Start-AIPScannerDiagnostics](https://docs.microsoft.com/powershell/module/azureinformationprotection/start-aipscannerdiagnostics?view=azureipps). Wenn Sie diesen Befehl ausführen, werden Protokolle generiert, die Sie in Ihre Falldetails hochladen können, wenn Sie ein Supportticket erstellen müssen.

1. Weitere Informationen zur Problembehandlung finden Sie [unter Troubleshooting your unified labeling on-premises scanner deployment](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner-tsg).

Wenn nach Abschluss dieser Schritte Probleme auftreten, exportieren Sie die Scannerprotokolle, und fügen Sie sie Ihrem [Supportticket](https://ms.portal.azure.com/#view/Microsoft_Azure_Support/HelpAndSupportBlade/~/overview) hinzu.

**Hinweis**: Sie können Ihre Protokolle mithilfe von PowerShell exportieren. Weitere Informationen finden Sie unter [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

Ressourcen:

- [Bereitstellen des Azure Information Protection-Scanners zum automatischen Klassifizieren und Schützen von Dateien](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)

- [Angeben und Verwenden des Token-Parameters für Set-AIPAuthentication](https://docs.microsoft.com/previous-versions/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)

- [Ausführen eines Suchzyklus und Anzeigen von Berichten für den Scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)

- [Azure Information Protection-Dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)

- [Anforderungen für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/requirements)

- [Herunterladen des Azure Information Protection-Clients](https://www.microsoft.com/download/details.aspx?id=53018)

Ressourcen für Scanner-DLP:

- [Informationen zum lokalen Microsoft 365-Scanner zur Verhinderung von Datenverlust](https://docs.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-learn)

- [Erste Schritte mit dem lokalen Scanner zur Verhinderung von Datenverlust](https://docs.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-get-started)

- [Verwenden des lokalen Microsoft 365-Scanners zur Verhinderung von Datenverlust](https://docs.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-use)