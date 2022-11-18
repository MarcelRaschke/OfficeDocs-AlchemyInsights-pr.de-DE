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
ms.custom:
- "6700003"
- "979"
ms.date: 08/16/2022
ms.openlocfilehash: 486fef72946f255042448f0289b8b7fc70fdae02
ms.sourcegitcommit: c524d66c406fcb7c0de677d2aa465e04e4f5553a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/16/2022
ms.locfileid: "67358304"
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

Um Email (Exchange Online) vor dem Zugriff durch nicht kompatible Geräte zu schützen, müssen beide Dokumente befolgt werden:

1. [Schützen des E-Mail-Zugriffs von Geräten mithilfe von EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Schützen des E-Mail-Zugriffs von Geräten mit modernen Authentifizierungsclients wie Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)