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
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 935f2b2780ce1f6662235e9c6a6e71db42da21d4
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62752908"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an

Berichte im Microsoft 365 Admin Center zeigen keine Benutzernamen an, sondern Alpha-Numerische Werte wie B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dies ist das erwartete Verhalten und wurde im Nachrichtencenter kommuniziert (MC275344, veröffentlicht am 3. August 2021). 

Globale Administratoren können diese Änderung für ihren Mandanten rückgängig machen und identifizierbare Benutzerinformationen anzeigen, wenn die Datenschutzpraktiken ihrer Organisation dies zulassen. Um die Änderung für den Mandanten rückgängig zu machen:

1. Wechseln Sie im Admin Center zu **Einstellungen** > **Organisationseinstellungsdienste,** > [**Dienste**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) und wählen Sie **Berichte** aus. 
1. Wählen Sie unter **Auswählen, wie Benutzerinformationen angezeigt werden sollen** die Option **Identifizierbare Benutzerinformationen in Berichten anzeigen** aus, und führen Sie dann den Bericht erneut aus.