---
title: Erstellen einer Organisationsbeziehung, um es Ihren Benutzern zu ermöglichen, mit einer anderen Organisation zusammenzuarbeiten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9a8fe3c754e6e5db8cd8daf8d58a3538cb11585e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63239777"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>Erstellen einer Organisationsbeziehung, um es Ihren Benutzern zu ermöglichen, mit einer anderen Organisation zusammenzuarbeiten

1. Wechseln Sie vom Microsoft 365 Admin Center-Dashboards zu **Admin** > **Exchange**.
2. Wechseln Sie zu **Organisation** > **Freigabe**.
3. Klicken Sie unterhalb von **Organisationsfreigabe** auf **Neu**.
4. Geben Sie im Bereich **Neue Organisationsbeziehung** im Feld **Beziehungsname** einen Anzeigenamen für die Organisationsbeziehung ein.
5. Geben Sie im Feld **Domäne für Freigabe** die Domäne für die externe Office 365- oder lokale Exchange-Organisation ein, die Einsicht in die Kalender haben soll. Wenn Sie mehr als eine Domäne eingeben müssen, trennen Sie die Domänennamen mit einem Komma. Beispiel: contoso.com, service.contoso.com.
6. Aktivieren Sie das Kontrollkästchen **Freigabe von Frei/Gebucht-Kalenderinformationen aktivieren**, um die Kalenderfreigabe mit den angegebenen Domänen zu ermöglichen. Legen Sie die Freigabeebene für Frei/Gebucht-Kalenderinformationen fest und definieren Sie, welche Benutzer Frei/Gebucht-Kalenderinformationen freigeben können.  

Wählen Sie eine der folgenden Optionen zur Festlegung der Frei/Gebucht-Zugriffsebene:

- **Frei/Gebucht-Kalenderinformationen nur mit Zeit**
- **Frei/Gebucht-Kalenderinformationen mit Zeit, Betreff und Ort**  

 Um festzulegen, welche Benutzer die Frei/Gebucht-Kalenderinformationen freigeben können, wählen Sie eine der folgenden Optionen aus:

- **Jeder in Ihrer Organisation**
- **Eine bestimmte Sicherheitsgruppe**  

Klicken Sie auf **Durchsuchen**, um eine Sicherheitsgruppe aus der Liste auszuwählen, und klicken Sie dann auf **OK**.

Klicken Sie auf **Speichern**, um die Organisationsbeziehung zu erstellen.  

**Hinweis:** Bei mandantenübergreifenden Konfigurationen werden persönliche Kontakte für die Frei/Gebucht-Suche nicht unterstützt. Die Kontakte müssen in die globale Adressliste aufgenommen werden, damit die Frei/Gebucht-Suche durchgeführt werden kann.

**Für vollständige Informationen zu diesem Thema lesen Sie:**

- [Erstellen einer Organisationsbeziehung in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [Ändern einer Organisationsbeziehung in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [Entfernen einer Organisationsbeziehung in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
