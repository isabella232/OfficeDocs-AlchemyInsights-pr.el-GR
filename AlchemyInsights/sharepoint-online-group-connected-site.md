---
title: Προσθήκη ομάδας σε τοποθεσία του SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912966"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ζητήματα κατά τη δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας στο SharePoint

1. Ορισμένα συνηθισμένα ζητήματα που παρουσιάστηκαν κατά τη δημιουργία ή την εκ νέου δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας.
Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

   - Λήψη [κελύφους διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το Powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Καταργήστε την τοποθεσία από τις διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet Powershell [κατάργησης-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Το Powershell απαιτείται για τη μόνιμη διαγραφή τοποθεσιών ομάδας.

1. Εάν δημιουργείτε μια συνδεδεμένη ομάδα τοποθεσίακαι λαμβάνετε μια προειδοποίηση: **Υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, ελέγξτε τις υπάρχουσες ομάδες από το Κέντρο [διαχείρισης του Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Για να επιλύσετε το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με διαφορετικό ψευδώνυμο.

1. Υπάρχουν διάφοροι τρόποι δημιουργίας και χρήσης σύγχρονων ομάδων με το SharePoint.

   - Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα Microsoft 365. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Σύνδεση μιας ομάδας του Microsoft 365 χρησιμοποιώντας το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας Microsoft 365, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).
