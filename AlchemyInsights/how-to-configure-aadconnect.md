---
title: 646 Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1300023"
- "646"
ms.date: 04/21/2020
ms.openlocfilehash: 79a6358681c50469009caec733fba551b357aa3d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66297512"
---
# <a name="configure-sync-features"></a>Konfigurieren von Synchronisierungsfeatures

Azure AD Connect enthält mehrere Features, die standardmäßig aktiviert sind oder die Sie später aktivieren können. Einige Features erfordern eine zusätzliche Konfiguration in bestimmten Umgebungen.

- [Filtergrenzwerte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) , die die Objekte mit Azure AD synchronisiert werden. Standardmäßig werden alle Benutzer, Kontakte, Gruppen und Windows 10 Computerkonten synchronisiert. Sie können Objekte basierend auf Domänen, OUs oder anderen Attributen ein- oder ausschließen.

- [Die Kennworthashsynchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronisiert den Kennworthash vom lokales Active Directory mit Azure AD. Dies ermöglicht die Kennwortverwaltung an einem Ort, aber die Verwendung desselben Kennworts sowohl in lokalen als auch in Cloudumgebungen. Da Active Directory die autorisierende Quelle ist, können Sie Ihre eigenen Kennwortrichtlinien verwenden.

- [Mit der Self-Service-Kennwortzurücksetzung (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) können Benutzer ihre eigenen Kennwörter in der Cloud zurücksetzen und gleichzeitig Ihre lokale Kennwortrichtlinie anwenden.

- [Das Geräterückschreiben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ermöglicht es registrierten Geräten in Azure AD, in die lokales Active Directory zurückgeschrieben zu werden, sodass sie für bedingten Zugriff verwendet werden können.

- [Verhindern von versehentlichen Löschvorgängen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ist standardmäßig aktiviert, um zu viele gleichzeitige Objektlöschungen zu verhindern (mehr als 500 Objekte pro Synchronisierung). Sie können diese Einstellung so ändern, dass sie den Anforderungen Ihrer Organisation entspricht.

- [Das automatische Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist standardmäßig für Expressinstallationen aktiviert und trägt dazu bei, dass Ihre Version von Azure AD Connect immer aktuell ist.
