---
title: Setup-Pop-Imap
ms.author: v-ftangonan
author: IpeTangonan
manager: anita.danford
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9009992"
- "17102"
ms.date: 04/15/2022
ms.openlocfilehash: 4f53229c7575f5023e2dccd9f81f3f1b4e3c8279
ms.sourcegitcommit: b4b034cf2e51e500744c03e8dcbeba5ab9ab9d7e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/16/2022
ms.locfileid: "64892027"
---
# <a name="setup-popimap4"></a>Einrichten von POP/IMAP4

Nachdem Sie den POP3- und IMAP4-Clientzugriff aktiviert haben, müssen Sie den Benutzern die Informationen in der folgenden Tabelle bereitstellen, damit sie ihre E-Mail-Programme mit ihren Exchange Online Postfächern verbinden können.

POP3- und IMAP4-E-Mail-Programme verwenden zum Versenden von Nachrichten an den E-Mail-Server weder POP3 noch IMAP4. E-Mail-Programme, die POP3 und IMAP4 verwenden, versenden Nachrichten mit dem SMTP-Protokoll.

| Protokoll | Servername | Port | Verschlüsselungsmethode |
|---|---|---|---|
| POP3 | Outlook.office365.com | 995 | SSL/TLS |
| IMAP4 | Outlook.office365.com | 993 | SSL/TLS |
| SMTP | Smtp.office365.com | 587 | STARTTLS |

Weitere Informationen zu POP3 und IMAP4 in Exchange Online finden Sie unter [POP3 und IMAP4 in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/pop3-and-imap4/pop3-and-imap4).

Wir sind für Sie da, wenn Sie weitere Unterstützung benötigen. Um sich **mit einem Microsoft-Spezialisten** für weitere Hilfe zu verbinden, wählen Sie einen Chat mit einem Microsoft-Spezialisten aus, und **klicken Sie unten auf "Live-Chat** ".
