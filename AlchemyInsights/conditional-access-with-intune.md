---
title: Bedingter Zugriff mit Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 55d4eb2bffbc1703e77aea2010307b67a3010958
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62557372"
---
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit Intune

Für die Verwendung des  **bedingten Zugriffs**  mit Intune sind drei Schritte erforderlich:

- Erstellen Sie eine **Compliancerichtlinie** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)[, Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt werden müssen, bevor das Gerät als kompatibel betrachtet wird. Beispielsweise muss ein Gerät über einen Pin mit mindestens 6 Ziffern verfügen, bevor es als kompatibel betrachtet wird.
- Erstellen Sie eine **Richtlinie für bedingten Zugriff**  , die definiert, welche Ressourcen geschützt werden und welche Bedingungen für den Zugriff auf diese Ressourcen erfüllt sein müssen.  [Beispielsweise](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  muss ein Gerät vor dem Zugriff auf Unternehmens-E-Mails konform sein.
- Stellen Sie sicher, dass sowohl **Compliancerichtlinien**  als auch  **Richtlinien für bedingten Zugriff**  auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.

**Nützliche Links:**

[Übersicht über die Gerätekompatibilität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung durch Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Um E-Mails (Exchange online) vor dem Zugriff durch nicht konforme Geräte zu schützen, müssen beide Dokumente befolgt werden:

1. [Schützen des E-Mail-Zugriffs von Geräten mit EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Schützen des E-Mail-Zugriffs von Geräten mithilfe moderner Authentifizierungsclients wie Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)