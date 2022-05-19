---
title: Vertraulichkeitsbezeichnungen werden nicht angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: eb161cc7525e18c7731c44e98cf4adc092deab10
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65588043"
---
# <a name="sensitivity-labels-not-appearing"></a>Vertraulichkeitsbezeichnungen werden nicht angezeigt

Vertraulichkeitsbezeichnungen ermöglichen Es Ihnen, Ihre vertraulichen Inhalte zu klassifizieren und zu schützen. Sie können im Microsoft Purview-Complianceportal, Microsoft 365 Security Center oder Microsoft 365 Security & Compliance Center unter Klassifizierung > Vertraulichkeitsbezeichnungen erstellt werden. Weitere Informationen zu diesem Feature finden Sie [unter Übersicht über Vertraulichkeitsbezeichnungen](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Wenn Sie Ihre Vertraulichkeitsbezeichnungen konfiguriert haben, diese aber nicht in den Microsoft 365-Apps angezeigt werden, überprüfen Sie Folgendes:

- Vergewissern Sie sich, dass die Vertraulichkeitsbezeichnung für die gewünschten Benutzer und Gruppen [veröffentlicht](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) wurde.

- Vergewissern Sie sich, dass der Benutzer eine App verwendet, die Vertraulichkeitsbezeichnungen unterstützt . Weitere Informationen finden Sie [unter Vertraulichkeitsbezeichnungen in Ihrem Dokument](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Wenn Sie [Azure Information Protection Bezeichnungen migrieren](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), beachten Sie die [hier](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels) aufgeführten Überlegungen.

- Unterstützung der Verhinderung von Datenverlust (Data Loss Prevention, DLP): Derzeit können nur Aufbewahrungsbezeichnungen als Bedingung in DLP-Richtlinien verwendet werden.  Unterstützung für Vertraulichkeitsbezeichnungen in einer DLP-Richtlinie ist noch nicht verfügbar, aber wir arbeiten daran.

- Wenn die Verschlüsselung für eine Vertraulichkeitsbezeichnung aktiviert ist, können Sie eine der folgenden Optionen auswählen:
    - Berechtigungen sofort zuweisen
    - Benutzern die Zuweisung von Berechtigungen überlassen


Weitere Informationen zu möglichen Problemen finden Sie unter [Bekannte Probleme mit Vertraulichkeitsbezeichnungen](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).