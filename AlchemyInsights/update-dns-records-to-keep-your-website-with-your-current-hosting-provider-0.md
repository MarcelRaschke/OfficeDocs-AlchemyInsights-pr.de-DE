---
title: Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 0e2ecc4a3169d5d4129595ea8c5af1c92282c6c2
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66011949"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen

1. Wechseln Sie im Microsoft 365 Admin Center zur Seite **"Domänen einrichten** > ", und wählen Sie in der Liste der Domänen die Domäne aus, die Sie für Ihre Website verwenden.[](https://admin.microsoft.com/AdminPortal/Home?ref=Domains)

2. Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:

  - Geben Sie unter **DNS-Typ** ein: **A (Adresse)**

  - Geben Sie unter **Hostname oder Alias** Folgendes ein: **@**

  - Geben Sie unter **IP-Adresse** die statische IP-Adresse für Ihre Website ein, unter der diese derzeit gehostet wird, beispielsweise "172.16.140.1".

    Es muss eine  *statische*  IP-Adresse für die Website sein, keine  *dynamische*  . Überprüfen Sie bei der Website, auf der Ihre Website gehostet wird, dass Sie eine statische IP-Adresse für Ihre öffentliche Website erhalten können.

3. Klicken Sie auf **Speichern**.

Darüber hinaus können Sie einen CNAME-Eintrag erstellen, damit Kunden Ihre Website besser finden können.
  
1. Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:

  - Geben Sie unter **DNS-Typ** ein: **CNAME (Alias)**

  - Geben Sie unter **Hostname oder Alias** Folgendes ein: **www**

  - Geben Sie unter **Verweist auf die Adresse** den vollqualifizierten Domänennamen (Fully Qualified Domain Name, FQDN) Ihrer Website ein, beispielsweise contoso.com.

2. Wählen Sie **Speichern**.
