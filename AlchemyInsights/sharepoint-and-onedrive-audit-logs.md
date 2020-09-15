---
title: Κλασικές αναφορές αρχείου καταγραφής ελέγχου του SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662208"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Αρχεία καταγραφής ελέγχου του SharePoint Classic

Ο έλεγχος παλαιού τύπου SPO μετεγκαταστάθηκε σε ενοποιημένο αρχείο καταγραφής ελέγχου (UAL). Όλες οι αναφορές ελέγχου παλαιού τύπου SPO θα τροφοδοτούνται πλέον μέσω του UAL και τα σήματα ελέγχου παλαιού τύπου έχουν μετεγκατασταθεί στο UAL.

Βασικές αλλαγές:

* Η περικοπή δεν είναι διαθέσιμη ως δυνατότητα.
* Η επιλογή συγκεκριμένων συμβάντων για έλεγχο δεν είναι διαθέσιμη. Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγμένων συμβάντων που είναι διαθέσιμα από προεπιλογή.
* Η επιλογή " **θέση** " στην περιοχή " **ΠΡΟΣΑΡΜΟΣΜΈΝΕς αναφορές** " δεν είναι διαθέσιμη.
* Η επιλογή " **Άνοιγμα ή λήψη συμβάντων εγγράφων** " δεν είναι διαθέσιμη.

[Ρύθμιση παραμέτρων των ρυθμίσεων ελέγχου για μια συλλογή τοποθεσιών](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Αρχεία καταγραφής σύγχρονων ενοποιημένων ελέγχων του SharePoint και του OneDrive από τη συμμόρφωση

* [Ενεργοποίηση/απενεργοποίηση της ενοποιημένης καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Δεν απαιτείται πρόσθετη ρύθμιση παραμέτρων μέσα από το SharePoint ή το OneDrive.

Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, των φακέλων ή των χρηστών, των δικαιωμάτων:

* [Δραστηριότητες αρχείων και σελίδων](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Δραστηριότητες φακέλου](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Δραστηριότητες αίτησης για κοινή χρήση και πρόσβαση](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Δραστηριότητες συγχρονισμού](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Δραστηριότητες διαχείρισης τοποθεσίας](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε [στο θέμα Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
