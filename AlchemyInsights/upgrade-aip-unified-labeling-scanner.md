---
title: Upgrade des AIP-Scanners für einheitliche Bezeichnungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002282"
- "5535"
ms.openlocfilehash: 6e579bba31662448586311e50bde114d91566f87
ms.sourcegitcommit: fd40ab0f1a1d678e25c5165e8f4612919d72e9b5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/03/2022
ms.locfileid: "68326013"
---
# <a name="upgrading-the-aip-unified-labeling-scanner"></a>Upgrade des AIP-Scanners für einheitliche Bezeichnungen

Wenn Sie ein Upgrade des Microsoft Purview Information Protection Scanners/AIP-Scanners (einheitliche Version) durchführen, laden Sie die [neueste Version des Clients für einheitliche Bezeichnungen](https://www.microsoft.com/download/details.aspx?id=53018) herunter, und installieren Sie sie.

Upgradeschritte finden Sie [unter Upgrade des Azure Information Protection-Scanners (vereinheitlicht).](https://learn.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)

So beheben Sie häufige Bereitstellungsprobleme:

- Generieren Sie Protokolle, die Sie in die Falldetails hochladen können, wenn Sie ein Supportticket erstellen müssen, indem [Sie Start-AIPScannerDiagnostics](https://docs.microsoft.com/powershell/module/azureinformationprotection/start-aipscannerdiagnostics?view=azureipps) ausführen.
- Sehen Sie sich das Video [zum Installieren des lokalen Scanners an (7:41)](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/mip-scanner-deployment-watch-our-video/ba-p/2023277?attachment-id=32620).
- Stellen Sie sicher, dass Ihr Scannerbenutzer [über Superbenutzerberechtigungen verfügt](https://docs.microsoft.com/azure/information-protection/configure-super-users).
- Stellen Sie sicher, dass das Scannerkonto zur Richtlinienkonfiguration hinzugefügt wurde.

**Hinweis**: Um Ihre Protokolle über PowerShell zu exportieren, verwenden Sie [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

Ausführliche Informationen zur Problembehandlung finden Sie [unter Problembehandlung bei der bereitstellung des lokalen Scanners für einheitliche Bezeichnungen](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner-tsg).

Weitere Ressourcen finden Sie unter:

- [Was ist Azure Information Protection?](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bereitstellen des Azure Information Protection-Scanners und Ausführen eines Ermittlungszyklus](https://learn.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angeben und Verwenden des Token-Parameters für Set-AIPAuthentication](https://learn.microsoft.com/previous-versions/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Azure Information Protection – Anforderungen](https://learn.microsoft.com/azure/information-protection/requirements)
- [Powershell-Unterstützung für getrennte Scannerserver](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history#powershell-support-for-disconnected-scanner-servers)
- [Herunterladen des Azure Information Protection-Clients](https://www.microsoft.com/download/details.aspx?id=53018)

Informationen zu Scanner-DLP-Ressourcen finden Sie unter:

- Informationen zum lokalen Scanner finden [Sie unter Informationen zum lokalen Scanner zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-learn).
- Informationen zu den ersten Schritte mit dem Scanner finden [Sie unter "Erste Schritte mit dem lokalen Scanner zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-get-started)".
- Informationen zur Verwendung des lokalen Microsoft 365-Scanners zur Verhinderung von Datenverlust finden [Sie unter Verwenden des lokalen Scanners zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-use). 

Wenden Sie sich an die [Hilfe und den Support](https://ms.portal.azure.com/#view/Microsoft_Azure_Support/HelpAndSupportBlade/~/overview), um Unterstützung vom Azure-Portal zu erhalten. 