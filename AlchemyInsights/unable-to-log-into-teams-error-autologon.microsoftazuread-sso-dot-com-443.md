---
title: Die Anmeldung bei Teams ist aufgrund des Fehlers „autologon.microsoftazuread-sso.com:443“ nicht möglich.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038399"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Die Anmeldung bei Teams ist aufgrund des Fehlers „autologon.microsoftazuread-sso dot com:443“ nicht möglich.

Wenn das nahtlose einmalige Anmelden als O365-Authentifizierung aktiviert ist, muss die URL "autologon.microsoftazuread-sso.com" möglicherweise zu den Intranetsites hinzugefügt werden.  Wenn es zuvor zu vertrauenswürdigen Websites hinzugefügt wurde und nahtloses einmaliges Anmelden verwendet wird, sollte es aus den vertrauenswürdigen Websites entfernt werden.

Sehen Sie sich die Checkliste unter [Problembehandlung beim nahtlosen einmaligen Anmelden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist) an.

Befolgen Sie diese Schritte, um eine URL zur Liste der Intranetsites hinzuzufügen:

1. Öffnen Sie Internet Explorer, indem Sie auf die Schaltfläche **Start** klicken. Geben Sie im Suchfeld „Internet Explorer“ ein, und klicken Sie dann in der Liste der Ergebnisse auf **Internet Explorer**.
2. Klicken Sie auf **Extras**, und klicken Sie anschließend auf **Internetoptionen**.
3. Klicken Sie auf die Registerkarte **Sicherheit**.
4. Klicken Sie nun auf **Lokales Intranet** und dann auf die Schaltfläche **Sites** und auf **Erweitert**.
5. Geben Sie die Website-URL ein, und klicken Sie auf **Hinzufügen**.
6. Klicken Sie nach Abschluss des Vorgangs auf **Schließen**.

Weitere Informationen finden Sie unter [Dokumentation zur Bereitstellung von nahtlosem einmaligen Anmelden für O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (enthält den richtlinienbasierten Prozess zum Hinzufügen einer URL zu den Intranetsites in Schritt 3).
