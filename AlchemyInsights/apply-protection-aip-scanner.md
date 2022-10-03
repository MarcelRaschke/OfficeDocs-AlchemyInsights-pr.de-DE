---
title: Anwenden von Schutz mit Information Protection Scanner/AIP-Scanner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002280"
- "5504"
ms.openlocfilehash: b7a5810a53462d83686a920507c3807014aada07
ms.sourcegitcommit: fd40ab0f1a1d678e25c5165e8f4612919d72e9b5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/03/2022
ms.locfileid: "68325974"
---
# <a name="applying-protection-with-information-protection-scanneraip-scanner"></a>Anwenden von Schutz mit Information Protection Scanner/AIP-Scanner

Wenn Sie den Scanner ausführen, der mit dem Client für einheitliche Bezeichnungen installiert ist, beheben Sie häufige Bereitstellungsprobleme mit dem Information Protection Scanner/[AIP-Scanner, indem Sie Start-AIPScannerDiagnostics](https://docs.microsoft.com/powershell/module/azureinformationprotection/start-aipscannerdiagnostics?view=azureipps) ausführen. Mit diesem Befehl werden Protokolle generiert, die Sie in Ihre Falldetails hochladen können, wenn Sie ein [Supportticket](https://ms.portal.azure.com/#view/Microsoft_Azure_Support/HelpAndSupportBlade/~/overview) erstellen müssen.

Um Schutz anzuwenden, muss der Scannerbenutzer ein [Superbenutzer](https://docs.microsoft.com/azure/information-protection/configure-super-users) sein.  

Weitere Schritte zur Problembehandlung bei der lokalen Scannerbereitstellung finden Sie im [Handbuch zur Problembehandlung](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner-tsg).  

**Hinweis**: Wenn Sie derzeit nicht als Benutzer angemeldet sind, der den Scannerdienst ausführt, exportieren Sie Protokolle mit dem [Cmdlet "Export-AIPLogs -OnBehalfOf"](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

Informationen zum Konfigurieren des AIP-Scanners für die Anwendung von Klassifizierung und Schutz finden [Sie unter Konfigurieren des Scanners zum Anwenden von Klassifizierung und Schutz](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#configure-the-scanner-to-apply-classification-and-protection).

Weitere Ressourcen finden Sie unter:

- [Was ist Azure Information Protection?](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Wie Office-Anwendungen und -Dienste Azure Rights Management unterstützen](https://learn.microsoft.com/azure/information-protection/office-apps-services-support)
- [Anwendungen, die Azure Rights Management-Datenschutz unterstützen](https://learn.microsoft.com/azure/information-protection/requirements-applications) 
- [Azure Information Protection – Anforderungen](https://learn.microsoft.com/azure/information-protection/requirements)
- [Herunterladen des Azure Information Protection-Clients](https://www.microsoft.com/download/details.aspx?id=53018) 

Informationen zu Scanner-DLP-Ressourcen finden Sie unter:

- Informationen zum lokalen Scanner finden [Sie unter Informationen zum lokalen Scanner zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-learn).
- Informationen zu den ersten Schritte mit dem Scanner finden [Sie unter "Erste Schritte mit dem lokalen Scanner zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-get-started)".
- Informationen zur Verwendung des lokalen Microsoft 365-Scanners zur Verhinderung von Datenverlust finden [Sie unter Verwenden des lokalen Scanners zur Verhinderung von Datenverlust](https://learn.microsoft.com/microsoft-365/compliance/dlp-on-premises-scanner-use). 

Wenden Sie sich an die [Hilfe und den Support](https://ms.portal.azure.com/#view/Microsoft_Azure_Support/HelpAndSupportBlade/~/overview), um Unterstützung in der Azure-Portal zu benötigen. 