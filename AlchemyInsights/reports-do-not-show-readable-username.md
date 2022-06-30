---
title: Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9008619"
- "13809"
- "13810"
- "13812"
ms.date: 09/02/2021
ms.openlocfilehash: 129a16aede1c95ca8e0fd993f7c4e653b70ef20c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66399423"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an

Berichte im Microsoft 365 Admin Center zeigen keine Benutzernamen an, sondern Alpha-Numerische Werte wie B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dies ist das erwartete Verhalten und wurde im Nachrichtencenter kommuniziert (MC275344, veröffentlicht am 3. August 2021). 

Globale Administratoren können diese Änderung für ihren Mandanten rückgängig machen und identifizierbare Benutzerinformationen anzeigen, wenn die Datenschutzpraktiken ihrer Organisation dies zulassen. Um die Änderung für den Mandanten rückgängig zu machen:

1. Wechseln Sie im Admin Center zu **Einstellungen** > **Organisationseinstellungsdienste,** > [**Dienste**](https://admin.microsoft.com/Adminportal/Home?ref=Settings/Services) und wählen Sie **Berichte** aus. 
1. Wählen Sie unter **Auswählen, wie Benutzerinformationen angezeigt werden sollen** die Option **Identifizierbare Benutzerinformationen in Berichten anzeigen** aus, und führen Sie dann den Bericht erneut aus.