---
title: Ανάπτυξη προσθεμάτων για Εφαρμογές Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233526"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Ανάπτυξη προσθεμάτων για Εφαρμογές Microsoft 365

Η κεντρική ανάπτυξη είναι ο προτεινόμενος τρόπος για Office πρόσθετα σε χρήστες και ομάδες εντός του οργανισμού σας. Για να αναπτύξετε πρόσθετα, ακολουθήστε τα παρακάτω βήματα:

**Σημείωση:** Για να εγκαταστήσετε πρόσθετα για Office ως μεμονωμένο χρήστη, ανατρέξτε στο θέμα Προβολή, διαχείριση και εγκατάσταση προσθεμάτων [σε Office προγραμμάτων.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Επίσης, βεβαιωθείτε ότι η μεμονωμένη απόκτηση Office του Store είναι ενεργοποιημένη. Για λεπτομέρειες, ανατρέξτε στο θέμα Αποτροπή λήψεων προσθεμάτων απενεργοποιώντας το Office Store σε όλα τα [προγράμματα-πελάτες (εκτός Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Βεβαιωθείτε ότι το περιβάλλον σας πληροί τις απαιτήσεις για την ανάπτυξη προσθεμάτων χρησιμοποιώντας την Κεντρική ανάπτυξη. Για λεπτομέρειες, ανατρέξτε στο θέμα ["Απαιτήσεις".](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Μεταβείτε **Ρυθμίσεις**  >  **"Λήψη**  >  **εφαρμογών"** στο Microsoft 365 διαχείρισης για να αναπτύξετε πρόσθετα. 

Σημειώσεις: 

- Οι ενσωματωμένες εφαρμογές απαιτούν ο διαχειριστής να έχει δικαιώματα καθολικού διαχειριστή Exchange διαχειριστή.

- Κατά την ανάπτυξη προσθεμάτων σε πολλούς χρήστες, συνιστάται να κάνετε αναθέσεις εργασιών χρησιμοποιώντας ομάδες αντί για μεμονωμένους χρήστες. Για λεπτομέρειες, [ανατρέξτε στο θέμα "Ζητήματα" κατά την εκχώρηση ενός προσθέτου σε χρήστες και ομάδες.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Η κεντρική ανάπτυξη δεν υποστηρίζει χρήστες σε ένθετες ομάδες ή ομάδες που έχουν γονικές ομάδες. Για λεπτομέρειες, ανατρέξτε [στο θέμα Αναθέσεις εργασιών χρηστών και ομάδων.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Βεβαιωθείτε ότι η υπηρεσία διαχείρισης εφαρμογών του Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') είναι ενεργοποιημένη για να πραγματοποιήσουν είσοδο οι χρήστες. Για λεπτομέρειες, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων ιδιοτήτων εφαρμογής.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Εάν αντιμετωπίζετε προβλήματα με την ανάπτυξη προσθεμάτων χρησιμοποιώντας ενσωματωμένες εφαρμογές, δοκιμάστε να αναπτύξετε χρησιμοποιώντας [πρόσθετα.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

[Ανάπτυξη προσθεμάτων στο κέντρο διαχείρισης](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Διαχείριση προσθεμάτων στο κέντρο διαχείρισης](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Χρήση των cmdlet Του PowerShell κεντρικής ανάπτυξης για τη διαχείριση προσθεμάτων](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Δημοσίευση Office με χρήση της Κεντρικής ανάπτυξης μέσω του Microsoft 365 διαχείρισης](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Αντιμετώπιση προβλημάτων: Ο χρήστης δεν βλέπει πρόσθετα](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Αντιμετώπιση σφαλμάτων χρήστη με Office πρόσθετα](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)