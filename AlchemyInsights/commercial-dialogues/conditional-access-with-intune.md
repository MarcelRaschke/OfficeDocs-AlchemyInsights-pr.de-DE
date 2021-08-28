---
title: Verwenden des bedingten Zugriffs mit Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005773"
---
# <a name="using-conditional-access-with-intune"></a>Verwenden des bedingten Zugriffs mit Intune

Für die Verwendung des bedingten Zugriffs mit Intune sind drei Schritte erforderlich:

- [Erstellen Sie eine Compliancerichtlinie, um Einstellungen zu definieren, die erfüllt werden müssen, bevor das Gerät als kompatibel betrachtet wird. Beispielsweise muss ein Gerät über einen Pin mit mindestens 6 Ziffern verfügen, bevor es als kompatibel betrachtet wird.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Erstellen Sie eine Richtlinie für bedingten Zugriff, die definiert, welche Ressourcen geschützt werden und welche Bedingungen für den Zugriff auf diese Ressourcen erfüllt sein müssen. Beispielsweise muss ein Gerät vor dem Zugriff auf Unternehmens-E-Mails konform sein.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Stellen Sie sicher, dass sowohl Compliancerichtlinien als auch Richtlinien für bedingten Zugriff auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Weitere Informationen...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
