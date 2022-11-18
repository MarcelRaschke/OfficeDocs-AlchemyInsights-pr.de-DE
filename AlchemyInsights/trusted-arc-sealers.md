---
title: Vertrauenswürdige ARC-Dichtungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100029"
- "17752"
ms.date: 07/21/2022
ms.openlocfilehash: ec5955e41dc5ed68d1742cab82bdd5097915d47c
ms.sourcegitcommit: 4161edd5135b339311452742655d5f720953184e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/21/2022
ms.locfileid: "66930153"
---
# <a name="trusted-arc-sealers"></a>Vertrauenswürdige ARC-Dichtungen

Email Authentifizierungsmechanismen wie [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing), [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) und [DMARC](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dmarc-to-validate-email) werden verwendet, um die Absender von E-Mails auf die Sicherheit von E-Mail-Empfängern zu überprüfen, aber einige legitime Dienste nehmen Änderungen an der E-Mail zwischen Dem Absender und Empfänger vor. In Microsoft 365 Defender trägt ARC dazu bei, SPF-, DKIM- und DMARC-Zustellungsfehler aufgrund legitimer indirekter E-Mail-Flüsse zu reduzieren.

Vertrauenswürdige ARC-Sealer ist eine vom Administrator erstellte Liste von zwischengeschalteten Domänen, die arc-Abdichtung implementiert haben. Wenn eine E-Mail über einen vertrauenswürdigen ARC-Vermittler des Office 365 Mandanten an Office 365 weitergeleitet wird, überprüft Microsoft die ARC-Signatur und berücksichtigt basierend auf den ARC-Ergebnissen die bereitgestellten Authentifizierungsdetails.

Weitere Informationen finden Sie unter [Erstellen einer Liste vertrauenswürdiger ARC-Absender, um legitimen indirekten E-Mail-Nachrichtenflüssen zu vertrauen](https://go.microsoft.com/fwlink/?linkid=2201606).