---
title: Προσθήκη ομάδας σε τοποθεσία του SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771202"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ζητήματα κατά τη δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας στο SharePoint

1. Ορισμένα συνηθισμένα προβλήματα που παρουσιάζονται κατά τη δημιουργία ή την εκ νέου δημιουργία μιας συνδεδεμένης τοποθεσίας ομάδας.
Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

   - Λήψη [κελύφους διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το PowerShell, ανατρέξτε στο θέμα [γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Καταργήστε την τοποθεσία από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. Το PowerShell απαιτείται για τη μόνιμη διαγραφή τοποθεσιών ομάδας.

1. Εάν δημιουργείτε μια ομάδα συνδεδεμένη τοποθεσία και λαμβάνετε μια προειδοποίηση: **υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, επιλέξτε τις υπάρχουσες ομάδες από το [Κέντρο διαχείρισης του Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Για να επιλύσετε το πρόβλημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με ένα διαφορετικό ψευδώνυμο αντιστοιχισμένο.

1. Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.

   - Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Microsoft 365. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα σύνδεση μιας ομάδας Microsoft 365 με το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Για να δημιουργήσετε μια τοποθεσία Microsoft 365 που είναι συνδεδεμένη στην ομάδα, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).
