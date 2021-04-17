---
title: Erstellen einer Organisationsbeziehung, um es Ihren Benutzern zu ermöglichen, mit einer anderen Organisation zusammenzuarbeiten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816127"
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
