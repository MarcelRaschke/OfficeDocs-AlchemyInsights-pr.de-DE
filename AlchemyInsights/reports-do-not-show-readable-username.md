---
title: Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 8f26d2143a2062473dc032c9bf95253365baab3a
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66008890"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an

Berichte im Microsoft 365 Admin Center zeigen keine Benutzernamen an, sondern Alpha-Numerische Werte wie B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dies ist das erwartete Verhalten und wurde im Nachrichtencenter kommuniziert (MC275344, veröffentlicht am 3. August 2021). 

Globale Administratoren können diese Änderung für ihren Mandanten rückgängig machen und identifizierbare Benutzerinformationen anzeigen, wenn die Datenschutzpraktiken ihrer Organisation dies zulassen. Um die Änderung für den Mandanten rückgängig zu machen:

1. Wechseln Sie im Admin Center zu **Einstellungen** > **Organisationseinstellungsdienste,** > [**Dienste**](https://admin.microsoft.com/Adminportal/Home?ref=Settings/Services) und wählen Sie **Berichte** aus. 
1. Wählen Sie unter **Auswählen, wie Benutzerinformationen angezeigt werden sollen** die Option **Identifizierbare Benutzerinformationen in Berichten anzeigen** aus, und führen Sie dann den Bericht erneut aus.