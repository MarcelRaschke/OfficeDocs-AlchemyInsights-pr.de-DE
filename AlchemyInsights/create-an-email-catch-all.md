---
title: Erstellen eines E-Mail-Abfangs für alle
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 6402b56baa037b8599f2a9f7aec50edc721b8ea7
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65718117"
---
# <a name="create-an-email-catch-all"></a>Erstellen eines E-Mail-Abfangs für alle

Es wird dringend davon abgeraten, einen Fang zu verwenden. Es ist besser, dem Absender eine Unzustellbarkeit zurückzugeben, um absendern mitzuteilen, dass ihre Nachricht nicht als adressiert übermittelt werden konnte, damit sie Maßnahmen ergreifen können. Sie können das überwachte Postfach auch so einschränken, dass nur zuvor gültige E-Mail-Adressen abgefangen werden. 

Jede Erfassung des gesamten Postfachs empfängt viel Spam und kann schließlich ausgefüllt werden, wenn sie nicht genau überwacht wird. (Es gibt Empfangsgrenzwerte.) 

Wenn Sie fortfahren möchten, führen Sie die folgenden Schritte aus:

1. Erstellen Sie eine dynamische Verteilergruppe, & "Alle Empfängertypen" enthalten.

2. Erstellen Sie ein dediziertes Postfach zum Abfangen von E-Mails, z. B. catchall@domain.com.

3. Legen Sie für die bestimmte Domäne "DomainType" auf "InternalRelay" fest. Wenn Sie den Catch All später entfernen, stellen Sie sicher, dass die Domäne wieder auf "Autoritativ" festgelegt wird.

4. Erstellen Sie eine Mailflow-Transportregel wie folgt:

    - Wenn der Absender "Außerhalb der Organisation" ist
    - Umleiten der Nachricht an Catchall@domain.com
    - Außer wenn der Empfänger Mitglied von allusers@domain.com ist (Verteilergruppe enthält alle Mitglieder)
    - Überprüfen, ob neue Postfächer zur dynamischen Verteilergruppe hinzugefügt werden
