---
title: Bedingter Zugriff mit Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: eaf9c5444cd089aae6a9eaff1d2d4257a55f404a
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66413077"
---
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit Intune

Die Verwendung **des bedingten Zugriffs** mit Intune erfordert drei Schritte:

- Erstellen Sie eine  **Compliancerichtlinie**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt werden müssen, bevor das Gerät als konform betrachtet wird. Ein Gerät muss z. B. einen Pin mit mindestens 6 Ziffern aufweisen, bevor es als konform betrachtet wird.
- Erstellen Sie eine **Richtlinie für bedingten Zugriff**  , die definiert, welche Ressourcen geschützt werden und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zugreifen zu können.  [Beispielsweise](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  muss ein Gerät konform sein, bevor auf Unternehmens-E-Mails zugegriffen wird.
- Stellen Sie sicher, dass sowohl **Compliancerichtlinien**  als auch  **Richtlinien für bedingten Zugriff**  auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.

**Nützliche Links:**

[Übersicht über die Gerätecompliance](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Um E-Mail (Exchange Online) vor dem Zugriff durch nicht kompatible Geräte zu schützen, müssen beide Dokumente befolgt werden:

1. [Schützen des E-Mail-Zugriffs von Geräten mithilfe von EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Schützen des E-Mail-Zugriffs von Geräten mit modernen Authentifizierungsclients wie Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)