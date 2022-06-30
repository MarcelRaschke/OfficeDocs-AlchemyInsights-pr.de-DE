---
title: Verwenden des bedingten Zugriffs mit Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: a3a6c8b1970c4279ea56fa5db86dd07f48549f7d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66369435"
---
# <a name="using-conditional-access-with-intune"></a>Verwenden des bedingten Zugriffs mit Intune

Die Verwendung des bedingten Zugriffs mit Intune erfordert drei Schritte:

- [Erstellen Sie eine Compliancerichtlinie, um Einstellungen zu definieren, die erfüllt werden müssen, bevor das Gerät als konform betrachtet wird. Ein Gerät muss z. B. einen Pin mit mindestens 6 Ziffern aufweisen, bevor es als konform betrachtet wird.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Erstellen Sie eine Richtlinie für bedingten Zugriff, die definiert, welche Ressourcen geschützt werden und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zugreifen zu können. Beispielsweise muss ein Gerät konform sein, bevor auf Unternehmens-E-Mails zugegriffen wird.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Stellen Sie sicher, dass sowohl Compliancerichtlinien als auch Richtlinien für bedingten Zugriff auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Weitere Informationen...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
