---
title: Problem mit Attribut- und Bereichsdefinitionsfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 6cf090937b3ecf76e6e54243125d5f3912711ff6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62571807"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem mit Attribut- und Bereichsdefinitionsfilter

**Problem mit Konflikten zwischen UPN-Werten**

Die Workday zu AD-Benurtzerbereitstellung zeigt die Fehlermeldung **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** an. Der Vorgang ist fehlgeschlagen, weil der für das Hinzufügen/Ändern angegebene UPN-Wert nicht über die Gesamtstruktur hinweg eindeutig ist. Fehlerdetails: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

Der Wert **userPrincipalName**, den der Workday-Connector beim Erstellen des AD-Benutzerkontos festzulegen versucht, existiert in der AD-Zieldomäne bereits. Dies bedeutet, dass entweder (1) der Benutzer bereits vorhanden und die Prüfung der entsprechenden ID für den Benutzer fehlgeschlagen ist oder (2) die UPN-Generierungsregel einen Wert generiert hat, der einen Konflikt verursacht.

Folgende Lösungsschritte werden vorgeschlagen:

Wenn der Benutzer bereits vorhanden ist und die Prüfung der übereinstimmenden ID das Workday-Konto nicht mit dem Active Directory-Konto verknüpfen konnte, dann prüfen Sie, ob das übereinstimmende ID-Attribut (typischerweise **employeeID**) sowohl in Workday als auch in AD eine exakte Übereinstimmung aufweist. Wenn sie nicht übereinstimmen, handelt es sich um ein Datenproblem, das behoben werden muss. Wenn der EmployeeID-Wert in Workday beispielsweise 001052 und in AD 1052 lautet, kann das Bereitstellungsmodul die beiden Konten nicht miteinander verknüpfen und versucht, einen Benutzer zu erstellen, der bereits existiert. Die Lösung besteht in diesem Fall darin, den **EmployeeID**-Wert in AD so zu ändern, dass er die führenden Nullen enthält und somit 001052 lautet.
Wenn der die UPN erzeugende Ausdruck keinen eindeutigen Wert generiert, sollten Sie ggf. die Deduplizierungsfunktion **SelectUniqueValue** verwenden, damit jedes Mal ein eindeutiger Wert zu generiert wird.

**Workday zu AD-Benurtzerbereitstellung legt keinen Manager-Attributwert für AD-Benutzerkonto fest**

Der Auftrag „Workday zu AD-Benurtzerbereitstellung“ legt den Wert des **manager**-Attributs für AD-Benutzerkonten nicht fest. Es gibt zwei mögliche Szenarien, wenn dieses Verhalten auftritt:

1. Der Manager in Workday kann nicht in ein entsprechendes AD-Benutzerkonto aufgelöst werden, da der Manager nicht innerhalb der Bereichsdefinition liegt.
2. In einem Szenario mit **mehreren AD-Domänen** befindet sich der Manager in Workday nicht in der gleichen Domäne wie der Benutzer.

Probieren Sie die folgenden Schritte aus, um das Problem zu beheben:

1. Wenn Sie Bereichsdefinitionsfilter definiert haben, prüfen Sie zunächst, ob der Manager innerhalb der Bereichsdefinition liegt und die Bereichsdefinitionsklausel erfüllt. Wenn der Manager den Bereichsdefinitionsfilter nicht erfüllt, ändern Sie den Filter so, dass der Manager auch innerhalb der Bereichsdefinition des Bereitstellungsvorgangs liegt.
2. Wenn Sie über mehrere AD-Domänen verfügen, gilt für den Connector die bekannte Einschränkung, dass er domänenübergreifende Verweise auf Manager nicht auflösen kann.

Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













