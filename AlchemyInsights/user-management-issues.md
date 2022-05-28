---
title: Benutzerverwaltungsprobleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 72ef29e0ac33d9fc181ab396927c503bb04789cb
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65725801"
---
# <a name="user-management-issues"></a>Benutzerverwaltungsprobleme

**Was passiert mit den aktuell der Anwendung zugewiesenen Benutzern, wenn ich die Eigenschaft „Benutzerzuweisung erforderlich“ deaktiviere (setzen dieser Eigenschaft auf „Nein“)?**

Das Deaktivieren von **Benutzerzuweisung erforderlich** hat KEINEN Einfluss auf aktuell zugewiesene Benutzer. Das Deaktivieren dieser Eigenschaft wird einfach allen Benutzern erlauben, auf diese Anwendung zuzugreifen. Alle aufgelisteten Benutzer und Benutzer, die Gruppen in der Anwendung zugewiesen sind, bleiben weiterhin gültig.

- Informationen darüber, wie Sie Ihre App auf eine bestimmte Gruppe von Benutzern einschränken, finden Sie unter [Azure AD-App auf eine Gruppe von Benutzern einschränken – Microsoft Identity Platform | Microsoft-Dokumentation](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Informationen zum Zuweisen von Benutzern und Gruppen zu Unternehmensanwendungen im Azure Active Directory (Azure AD), entweder über das Azure-Portal oder mithilfe von PowerShell, finden Sie unter [Verwalten der Benutzerzuweisung für eine App im Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Informationen über die Delegation von Berechtigungen für die Anwendungserstellung und -Verwaltung finden Sie unter [Administratorberechtigungen für die Anwendungsverwaltung delegieren – Azure AD | Microsoft-Dokumentation](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).

- **Unternehmensapps für Benutzer ausblenden** – Verwenden Sie die folgenden Schritte, um alle Microsoft 365 Apps aus dem Bereich **MyApps** auszublenden. Die Apps werden im Office 365-Portal weiterhin ersichtlich sein.

  1. Melden Sie sich beim Azure-Portal als globaler Administrator für Ihr Verzeichnis an.
  2. Wählen Sie **Azure Active Directory** aus.
  3. Wählen Sie **Benutzer** aus.
  4. Wählen Sie **Benutzereinstellungen** aus.
  5. Klicken Sie unter **Unternehmensanwendungen** auf **Verwalten, wie Endbenutzer ihre Anwendungen starten und anzeigen**.
  6. Um **Benutzer können Office 365-Apps nur im Office 365-Portal anzeigen** zu aktivieren, klicken Sie auf **Ja**.
  7. Klicken Sie auf **Speichern**.
  8. Weitere Informationen finden Sie unter [Ausblenden einer Unternehmensanwendung aus der Erfahrung eines Benutzers in Azure AD | Microsoft-Dokumentation](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.).

- Wenn Sie eine SaaS (Software as a Service)-App für mehrere Organisationen anbieten, können Sie die App so konfigurieren, dass sie Anmeldungen von jedem Azure Active Directory (Azure AD)-Mandanten akzeptiert. Diese Konfiguration nennt sich „Ihre Anwendung multimandantenfähig machen“. Benutzer in einem beliebigen Azure AD-Mandanten können sich in Ihre App anmelden, nachdem Sie zugestimmt haben, ihr Konto mit Ihrer App zu verwenden. Weitere Informationen finden Sie unter [Apps erstellen, die Azure AD-Benutzer anmelden – Microsoft Identity Platform | Microsoft-Dokumentation](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Wie kann ein Endbenutzer auf die Anwendung zugreifen, nachdem er/sie der Anwendung zugewiesen ist?**

  Jede App im Unternehmensanwendungsblatt hat einen Link für den Zugriff von Endbenutzern. Benutzer können ebenfalls auf einfache Art und Weise über das **MyApps**-Portal auf die App zugreifen.

- **Möchten Sie wissen, welche Anwendungen und welche Art von Anwendungen Ihre Benutzer verwenden?**

  Sie können Anmeldeberichte für die letzten 30 Tage herunterladen von: **portal.azure.com** \> **Azure Active Directory** \> **Anmeldungen** \> **Bericht herunterladen**.

- Erfahren Sie, wie Sie [Einer Anwendung eine mandantenweite Administratorzustimmung erteilen](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) und [Konfigurieren, wie Endbenutzer Anwendungen zustimmen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Verstehen Sie, [wie die Zustimmung funktioniert](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) und [Verwalten Sie die Zustimmung für Anwendungen](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).
