---
title: Προσθήκη ομάδας σε μια τοποθεσία του SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750520"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Ζητήματα κατά τη δημιουργία ή την ομαδοποίηση συνδεδεμένων τοποθεσιών στο SharePoint Online

Υπάρχουν μερικά συνηθισμένα ζητήματα που παρουσιάστηκαν κατά τη δημιουργία ή την εκ νέου δημιουργία μιας ομάδας συνδεδεμένων τοποθεσιών.

 Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία της και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

Κατεβάστε το [κέλυφος διαχείρισης του Μπίσπο](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με PowerShell, δείτε [γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Κατάργηση της τοποθεσίας από διαγραμμένες τοποθεσίες χρησιμοποιώντας το cmdlet PowerShell [Διαγραφή τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Εάν δημιουργείτε μια τοποθεσία συνδεδεμένη σε ομάδα και λαμβάνετε μια προειδοποίηση μια άλλη ομάδα με το ίδιο ψευδώνυμο υπάρχει ήδη, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήστε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.

Υπάρχουν διαφορετικοί τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε σύγχρονες ομάδες με το SharePoint.

Μπορείτε να συνδέσετε υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365. Για περισσότερες πληροφορίες, ανατρέξτε [στο αρχείο σύνδεση μιας ομάδας του Office 365 χρησιμοποιώντας το χρήστη του SharePoint το ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία της ομάδας Office 365, θα πρέπει να δημιουργήσετε μια τοποθεσία ομάδας. Για περισσότερες πληροφορίες, ανατρέξτε [στο σημείο δημιουργία μιας τοποθεσίας ομάδας στο SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

