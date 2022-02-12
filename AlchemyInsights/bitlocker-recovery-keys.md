---
title: Bitlocker-Wiederherstellungsschlüssel
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: d9443a02899cecd654e773a23ff170d2a9a9ee72
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62580429"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Zugreifen auf Bitlocker-Wiederherstellungsschlüssel

Beim Konfigurieren von Bitlocker-Einstellungen intune Endpoint Protection Richtlinie ist es möglich, zu definieren, ob Bitlocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.

Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten einem Intune-Administrator als Teil des Blatts "Gerätedatensatz" auf dem Blatt "Intune-Geräte" auf zwei Arten angezeigt werden:

Geräte – Azure AD Geräte – > "Gerät" oder Geräte – > Alle Geräte – > "Gerät" – > Wiederherstellungsschlüssel

Wenn administrativer Zugriff auf das Gerät selbst besteht, kann der Wiederherstellungsschlüssel (Kennwort) auch angezeigt werden, indem Der folgende Befehl an einer Eingabeaufforderung mit erhöhten Rechten ausgeführt wird:

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
Wenn das Gerät vor der Registrierung in Intune verschlüsselt wurde, wurde der Wiederherstellungsschlüssel möglicherweise dem "Microsoft-Konto" (MSA) zugeordnet, das verwendet wurde, um sich während des OoBE-Prozesses beim Gerät anzumelden. Wenn dies der Fall war, sollten beim Zugriff auf  https://onedrive.live.com/recoverykey und der Anmeldung mit diesem MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.
 
Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, können die Wiederherstellungsinformationen im lokalen Active Directory gespeichert werden.

Wenn Sie die Endpunktschutzrichtlinie so konfiguriert haben, dass der Wiederherstellungsschlüssel in Azure Active Directory gespeichert wird, der Schlüssel für ein bestimmtes Gerät jedoch nicht hochgeladen wurde, können Sie den Upload auslösen, indem Sie den Wiederherstellungsschlüssel für dieses Gerät von der MEM-Konsole drehen. Ausführliche Informationen finden Sie unter [Drehen von BitLocker-Wiederherstellungsschlüsseln](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

