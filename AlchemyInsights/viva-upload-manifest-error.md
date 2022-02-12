---
title: Beheben Sie "Die Manifestdatei kann nicht gelesen werden. Versuchen Sie es später erneut." beim Hochladen von Viva Connections
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
- "9010305"
- "16343"
ms.date: 01/13/2022
ms.openlocfilehash: d94fe543b73ed459013e49ec291e00b7407f03aa
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62543482"
---
# <a name="resolve-we-cant-read-the-manifest-file-try-again-later-when-uploading-viva-connections"></a>Beheben Sie "Die Manifestdatei kann nicht gelesen werden. Versuchen Sie es später erneut." beim Hochladen von Viva Connections

Jede Manifestdatei für Viva Connections muss einen bestimmten Satz von Anforderungen erfüllen. Vor dem Hochladen des App-Pakets .zip muss die Manifestdatei den Manifestschemaanforderungen entsprechen.

Ausführliche Informationen finden Sie unter [Referenz: Manifestschema für Microsoft Teams](https://docs.microsoft.com/microsoftteams/platform/resources/schema/manifest-schema).

Hier sind die App-Paketanforderungen und die Zeichenbeschränkungen für die einzelnen:

- App-Symboldateien müssen im .PNG Format und 192 x 192 Pixel für das farbige Symbol und 32 x 32 Pixel für das Gliederungssymbol (monochrom) sein. Weitere Informationen finden Sie unter [App-Symbol](https://docs.microsoft.com/microsoftteams/platform/concepts/build-and-test/apps-package#app-icons).
- Alle Website-URLs sind erforderlich, um mit `https://`zu beginnen. Beispielsweise `https://contoso.sharepoint.com` die Startseite oder `https://www.contoso.com` die öffentliche Website der Organisation.
- Geben Sie den Namen der App so ein, wie sie in Teams angezeigt werden soll: (<= 30 Zeichen).  
- Geben Sie eine kurze Beschreibung für die App ein: (<= 80 Zeichen).  
- Geben Sie eine lange Beschreibung für die App ein: (<=4000 Zeichen).  
- Geben Sie den Organisationsnamen an: (<=30 Zeichen).  
