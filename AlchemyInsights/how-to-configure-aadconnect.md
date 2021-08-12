---
title: 646 Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963642"
---
# <a name="configure-sync-features"></a>Konfigurieren von Synchronisierungsfeatures

Azure AD Verbinden enthält mehrere Features, die standardmäßig aktiviert sind oder später aktiviert werden können. Einige Features erfordern eine zusätzliche Konfiguration in bestimmten Umgebungen.

- [Filtergrenzwerte,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) die die Objekte mit Azure AD synchronisiert werden. Standardmäßig werden alle Benutzer, Kontakte, Gruppen und Windows 10 Computerkonten synchronisiert. Sie können Objekte basierend auf Domänen, Organisationseinheiten oder anderen Attributen einschließen oder ausschließen.

- [Die Kennworthashsynchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronisiert den Kennworthash aus dem lokalen Active Directory mit Azure AD. Dies ermöglicht die Kennwortverwaltung an einem Ort, aber die Verwendung desselben Kennworts sowohl in lokalen als auch in Cloudumgebungen. Da Active Directory die autorisierende Quelle ist, können Sie Ihre eigenen Kennwortrichtlinien verwenden.

- [Die Self-Service-Kennwortzurücksetzung (Self-Service Password Reset, SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ermöglicht Es Benutzern, ihre eigenen Kennwörter in der Cloud zurückzusetzen und gleichzeitig Ihre lokale Kennwortrichtlinie anzuwenden.

- Mit dem [Geräterückschreiben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) können registrierte Geräte in Azure AD in das lokale Active Directory zurückgeschrieben werden, damit sie für bedingten Zugriff verwendet werden können.

- [Das Verhindern versehentlicher Löschungen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ist standardmäßig aktiviert, um zu viele gleichzeitige Objektlöschungen zu verhindern (mehr als 500 Objekte pro Synchronisierung). Sie können diese Einstellung an die Anforderungen Ihrer Organisation anpassen.

- [Das automatische Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist standardmäßig für Expressinstallationen aktiviert und trägt dazu bei, sicherzustellen, dass Ihre Version von Azure AD Verbinden immer aktuell ist.
