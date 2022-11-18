---
title: Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000247"
- "1834"
ms.date: 07/27/2020
ms.openlocfilehash: f978e25120d0de3ad3fd0199379c8c243fe3db21
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66350607"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität

**Mehrere Objekte**

Einer der häufigsten Gründe für diesen Fehler ist, dass eine Outlook Web Access-Anfrage nicht richtig weitergeleitet werden kann, wenn mehrere Objekte vorhanden sind, die dieselbe E-Mail-Adresse als Identität haben. Um diese Objekte zu finden, führen Sie die folgenden Befehle aus:

- `Get-Recipient <email address>`
- `Get-User <email address>`
- `Get-User <email address> -SoftDeletedUser`
- `Get-Contact <email address>`
- `Get-Mailbox <email address> -PublicFolder`
- `Get-Mailbox <email address> -IncludeSoftDeletedMailbox`
- `Get-Mailbox <email address> -InactiveMailboxOnly`

Um das Problem zu beheben, entfernen Sie mehrere Objekte mit derselben E-Mail-Identität, und stellen Sie sicher, dass es immer nur ein einziges Objekt mit einer bestimmten E-Mail-Identität gibt und dass sein Empfängertyp "UserMailbox" ist.

**Dieselbe Adresse wird für Postfächer von Unternehmen und Privatpersonen verwendet**

Eine weitere Ursache ist, wenn dieselbe Adresse für Postfächer von Unternehmen und Privatkunden verwendet wird. In diesem Fall muss der Benutzer seinen primären Verbraucheralias ändern, bis Cafe dieses Szenario unterstützt. Dies ist ein permanenter Fehler, der nicht ohne Intervention verschwindet.

Ausführliche Informationen finden Sie unter [Ändern der E-Mail-Adresse oder Telefonnummer für Ihr Microsoft-Konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).