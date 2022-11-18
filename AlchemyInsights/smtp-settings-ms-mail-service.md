---
title: SMTP-Einstellungen für den Microsoft 365-E-Mail-Dienst
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3000003"
- "12073"
ms.date: 07/26/2021
ms.openlocfilehash: 9adca7ab8744622598bdc04494f382414365748a
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66372675"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>SMTP-Einstellungen für den Microsoft 365-E-Mail-Dienst

Dies sind die SMTP-Einstellungen für die Microsoft 365-E-Mail-Dienste:

**Server**: smtp.office365.com </br>
**Port**: 587 </br>
**Verschlüsselung**: STARTTLS (nur TLS 1.2-Version wird jetzt unterstützt. Stellen Sie sicher, dass Ihre Anwendung oder Ihr Gerät TLS 1.2 unterstützt.) </br>
**Benutzername**: Ihre Office 365-E-Mail-Adresse (z. B. example@yourdomain.com) </br>
**Kennwort**: Ihr Office 365-Kennwort </br>
**Authentifizierung**: Erforderlich </br>
**Sendegrenzwerte**: 10.000 E-Mails pro Tag </br>

Informationen zu POP- und IMAP-Einstellungen finden Sie unter [POP-, IMAP- und SMTP-Einstellungen](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Informationen zu den verfügbaren Optionen zum Weiterleiten von E-Mails mithilfe von Microsoft 365 und den Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365 oder Office 365](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).