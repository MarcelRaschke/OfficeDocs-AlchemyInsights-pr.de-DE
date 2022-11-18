---
title: Konfigurieren des Diensts – AIP-Scanner (klassisch)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002277"
- "4991"
ms.openlocfilehash: c0be9cb9dd680a9db1977745ae0db5846d53e7ba
ms.sourcegitcommit: fd40ab0f1a1d678e25c5165e8f4612919d72e9b5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/03/2022
ms.locfileid: "68326016"
---
# <a name="configuring-the-service---aip-scanner-classic"></a>Konfigurieren des Diensts – AIP-Scanner (klassisch)

Lesen Sie die folgenden Empfehlungen, um den AIP-Scanner (klassisch) zu konfigurieren:

- Wenn Sie die [integrierten Informationstypen](https://learn.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) für Ihre Azure Information Protection -Richtlinie (AIP) verwendet haben, überprüfen Sie, ob Ihre Inhalte dem erwarteten Format entsprechen.
- Vergewissern Sie sich, dass die Bezeichnung ordnungsgemäß für **Automatisch** oder **Empfohlen** konfiguriert ist.

    **Hinweis:** **Die automatische** Bezeichnung ist für alle Office-Apps verfügbar. **Empfohlen** ist für alle Office-Apps mit Ausnahme von Outlook verfügbar.

- Vergewissern Sie sich, dass das für die Ausführung des Scanner-Diensts konfigurierte Benutzerkonto über Berechtigungen für den Zugriff auf alle konfigurierten Repositories verfügt. Weitere Informationen finden Sie unter [Konfigurieren von Superbenutzern für Azure Information Protection- und Discoverydienste oder Datenwiederherstellung](https://learn.microsoft.com/azure/information-protection/configure-super-users).

Wenn weiterhin Probleme auftreten, führen Sie die folgenden Schritte aus, um die AIP-Scannerprotokolle zu exportieren und zu sammeln:

1. Wechseln Sie unter dem Benutzerkontext, der den Scannerdienst ausführt, zu %localappdata%\Microsoft\MSIP.
1. Komprimieren Sie alle Inhalte im Ordner "MSIP".
1. Speichern Sie die Protokolle an einem beliebigen Ort, und fügen Sie sie an Ihre Serviceanfrage an.

Weitere Informationen zum Konfigurieren des AIP-Scanners finden Sie unter:

- [Was ist Azure Information Protection?](https://learn.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bereitstellen des Azure Information Protection-Scanners und Ausführen eines Ermittlungszyklus](https://learn.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angeben und Verwenden des Token-Parameters für Set-AIPAuthentication](https://learn.microsoft.com/previous-versions/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Azure Information Protection – Anforderungen](https://learn.microsoft.com/azure/information-protection/requirements)
- [Herunterladen des Azure Information Protection-Clients](https://www.microsoft.com/download/details.aspx?id=53018)

Wenden Sie sich an die [Hilfe und den Support](https://ms.portal.azure.com/#view/Microsoft_Azure_Support/HelpAndSupportBlade/~/overview), um Unterstützung in der Azure-Portal zu benötigen.