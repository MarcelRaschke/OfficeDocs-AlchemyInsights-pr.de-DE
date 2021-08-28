---
title: Erstellen eines E-Mail-Catch-All
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080745"
---
# <a name="create-an-email-catch-all"></a>Erstellen eines E-Mail-Catch-All

Von der Verwendung eines Catch all wird dringend abgeraten. Es empfiehlt sich, eine Rückmeldung an den Absender bereitzustellen, damit die Absender wissen, dass ihre Nachricht nicht als adressiert zugestellt werden konnte, damit sie Maßnahmen ergreifen können. Sie können das überwachte Postfach auch so einschränken, dass es nur zuvor gültige E-Mail-Adressen abfangen kann. 

Alle Catch-Postfächer erhalten ein großes Maß an Spam und füllen möglicherweise, wenn sie nicht genau überwacht werden. (Es gibt Empfangsgrenzwerte.) 

Wenn Sie fortfahren möchten, führen Sie die folgenden Schritte aus:

1. Erstellen Sie eine dynamische Verteilergruppe & "Alle Empfängertypen" enthalten.

2. Erstellen Sie ein dediziertes Postfach zum Abfangen von E-Mails, z. B. catchall@domain.com.

3. Legen Sie für die spezifische Domäne den DomainType auf "InternalRelay" fest. Wenn Sie später den Catch all entfernen, stellen Sie sicher, dass die Domäne wieder auf Autoritativ festgelegt ist.

4. Erstellen Sie wie folgt eine E-Mailflow-Transportregel:

    - Wenn der Absender "Außerhalb der Organisation" ist
    - Umleiten der Nachricht an Catchall@domain.com
    - Außer wenn der Empfänger Mitglied von allusers@domain.com ist (Verteilergruppe enthält alle Mitglieder)
    - Überprüfen Sie, ob neue Postfächer zur dynamischen Verteilergruppe hinzugefügt werden.
