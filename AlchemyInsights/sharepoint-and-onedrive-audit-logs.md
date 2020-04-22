---
title: Κλασικές αναφορές αρχείου καταγραφής ελέγχου του SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741965"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Κλασικά αρχεία καταγραφής ελέγχου του SharePoint

Ο έλεγχος παλαιού τύπου SPO μετεγκαταστάθηκε στο ενοποιημένο αρχείο καταγραφής ελέγχου (UAL). Όλες οι αναφορές ελέγχου παλαιού τύπου SPO θα τροφοδοτούνται τώρα μέσω UAL και τα σήματα ελέγχου παλαιού τύπου έχουν μετεγκατασταθεί σε UAL.

Βασικές αλλαγές:

* Η περικοπή ΔΕΝ είναι διαθέσιμη ως δυνατότητα.
* Η επιλογή συγκεκριμένων συμβάντων για έλεγχο ΔΕΝ είναι διαθέσιμη. Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγμένα συμβάντα που είναι διαθέσιμα από προεπιλογή.
* Η **επιλογή "Θέση"** στην περιοχή **Προσαρμοσμένες αναφορές** ΔΕΝ είναι διαθέσιμη.
* Η επιλογή **Άνοιγμα ή λήψη συμβάντων εγγράφων** ΔΕΝ είναι διαθέσιμη.

[Ρύθμιση παραμέτρων ελέγχου για μια συλλογή τοποθεσιών](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Αρχεία καταγραφής ενοποιημένου ελέγχου του SharePoint και του OneDrive (Unified Audit) του SharePoint και του OneDrive

* [Ενεργοποίηση/απενεργοποίηση ενοποιημένης καταγραφής ελέγχου](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Δεν απαιτείται πρόσθετη ρύθμιση παραμέτρων στο SharePoint ή το OneDrive.

Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, φακέλων, χρηστών, δικαιωμάτων:

* [Δραστηριότητες αρχείων και σελίδων](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Δραστηριότητες φακέλων](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Δραστηριότητες κοινής χρήσης και αίτησης πρόσβασης](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Δραστηριότητες συγχρονισμού](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Δραστηριότητες διαχείρισης τοποθεσίας](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε στο θέμα [Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
