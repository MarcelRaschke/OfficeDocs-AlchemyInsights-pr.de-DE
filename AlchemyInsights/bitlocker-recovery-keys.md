---
title: Bitlocker-Wiederherstellungsschlüssel
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000220"
- "1922"
ms.openlocfilehash: d8126044c5a961959855b8b0c474ec6e04cee47c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66311976"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Zugreifen auf Bitlocker-Wiederherstellungsschlüssel

Beim Konfigurieren von Bitlocker-Einstellungen Intune Endpoint Protection-Richtlinie kann definiert werden, ob Bitlocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.

Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten auf zwei Arten für einen Intune Administrator als Teil der Gerätedatensatzdaten auf Intune Blatt "Geräte" sichtbar sein:

Geräte – Azure AD-Geräte -> "Gerät" ODER Geräte -> Alle Geräte -> "Gerät" -> Wiederherstellungsschlüssel

Wenn administratorgesteuerter Zugriff auf das Gerät selbst besteht, kann der Wiederherstellungsschlüssel (Kennwort) durch Ausführen des folgenden Befehls an einer Eingabeaufforderung mit erhöhten Rechten angezeigt werden:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Wenn das Gerät vor der Registrierung in Intune verschlüsselt wurde, wurde der Wiederherstellungsschlüssel möglicherweise mit dem "Microsoft-Konto" (MSA) verknüpft, das für die Anmeldung beim Gerät während des OoBE-Prozesses verwendet wurde. Wenn dies der Fall war, sollten beim Zugriff  https://onedrive.live.com/recoverykey auf und anmelden mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.
 
Wenn das Gerät aufgrund der Konfiguration über domänenbasierte Gruppenrichtlinien verschlüsselt wurde, werden die Wiederherstellungsinformationen möglicherweise im lokalen Active Directory gespeichert.

Wenn Sie die Endpoint Protection-Richtlinie so konfiguriert haben, dass der Wiederherstellungsschlüssel in Azure Active Directory gespeichert wird, der Schlüssel für ein bestimmtes Gerät jedoch nicht hochgeladen wurde, können Sie den Upload auslösen, indem Sie den Wiederherstellungsschlüssel für dieses Gerät über die MEM-Konsole drehen. Ausführliche Informationen finden Sie [unter "Drehen von BitLocker-Wiederherstellungsschlüsseln"](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

