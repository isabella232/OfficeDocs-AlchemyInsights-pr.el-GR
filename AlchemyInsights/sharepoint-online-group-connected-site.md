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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770351"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ζητήματα κατά τη δημιουργία μιας ομάδας συνδεδεμένη τοποθεσία στο SharePoint

1. Ορισμένα συνηθισμένα ζητήματα που παρουσιάζονται κατά τη δημιουργία ή την εκ νέου δημιουργία μιας ομάδας συνδεδεμένης τοποθεσίας.
Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε μόνιμα την προηγούμενη τοποθεσία.

   - Κατεβάστε το [κέλυφος διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Για περισσότερες πληροφορίες σχετικά με τα γρήγορα αποτελέσματα με το PowerShell, δείτε [γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Καταργήστε την τοποθεσία από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet [Κατάργηση-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. Απαιτείται PowerShell για τη μόνιμη διαγραφή τοποθεσιών ομάδας.

1. Εάν δημιουργείτε μια ομάδα συνδεδεμένη τοποθεσία και λαμβάνετε μια προειδοποίηση: **υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο**, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το κέντρο διαχείρισης](https://admin.microsoft.com/AdminPortal/Home#/groups). Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με ένα διαφορετικό ψευδώνυμο αντιστοιχισμένο.

1. Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.

   - Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365. Για περισσότερες πληροφορίες, ανατρέξτε [στο σημείο σύνδεση μιας ομάδας του Office 365 χρησιμοποιώντας το περιβάλλον εργασίας χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία του Office 365 Group, θα πρέπει να δημιουργήσετε μια [τοποθεσία ομάδας](https://admin.microsoft.com/sharepoint).
