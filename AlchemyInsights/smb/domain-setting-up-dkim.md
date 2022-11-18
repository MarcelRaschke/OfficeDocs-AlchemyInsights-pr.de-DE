---
title: Einrichten von DKIM
ms.author: v-ftangonan
author: IpeTangonan
manager: anita.danford
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9009960"
- "17063"
ms.date: 04/15/2022
ms.openlocfilehash: fba100005d45cf89300cde8c5ca7137042690d6b
ms.sourcegitcommit: b4b034cf2e51e500744c03e8dcbeba5ab9ab9d7e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/16/2022
ms.locfileid: "64892107"
---
# <a name="setting-up-dkim"></a>Einrichten von DKIM

Mit DKIM können Sie ausgehenden E-Mail-Nachrichten in der Nachrichtenkopfzeile eine digitale Signatur hinzufügen. Wenn Sie DKIM konfigurieren, autorisieren Sie Ihre Domäne, ihren Namen einer E-Mail-Nachricht mithilfe der kryptografischen Authentifizierung zuzuordnen oder zu signieren.

Alle akzeptierten Domänen Ihres Mandanten werden im Microsoft 365 Defender Portal unter der DKIM-Seite angezeigt. Nachdem Ihre Domäne hinzugefügt wurde, führen Sie die folgenden Schritte aus, um DKIM zu konfigurieren.

1. Wählen Sie die Domäne aus, die Sie DKIM auf der DKIM-Seite ([https://security.microsoft.com/dkimv2](https://security.microsoft.com/dkimv2)) oder () konfigurieren möchten.[https://protection.office.com/dkimv2](https://protection.office.com/dkimv2)
2. Schieben Sie den Umschalter auf **"Aktivieren"**. Es wird ein Popupfenster angezeigt, das besagt, dass Sie CNAME-Einträge hinzufügen müssen.
3. Kopieren Sie die im Popupfenster angezeigten CNAMES.
4. Veröffentlichen Sie die kopierten CNAME-Einträge bei Ihrem DNS-Dienstanbieter.
5. Kehren Sie zur DKIM-Seite zurück, um DKIM zu aktivieren.

Weitere Informationen finden Sie unter [Verwenden von DKIM für E-Mails in Ihrer benutzerdefinierten Domäne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Wir sind für Sie da, wenn Sie weitere Unterstützung benötigen. Um sich **mit einem Microsoft-Spezialisten** für weitere Hilfe zu verbinden, wählen Sie einen Chat mit einem Microsoft-Spezialisten aus, und **klicken Sie unten auf "Live-Chat** ".
