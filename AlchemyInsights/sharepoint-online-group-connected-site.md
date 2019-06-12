---
title: Προσθήκη μιας ομάδας σε μια τοποθεσία του SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758731"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Δημιουργία ομάδας συνδεδεμένη τοποθεσία στο SharePoint Online

Υπάρχουν μερικά κοινά θέματα που προέκυψαν κατά τη δημιουργία ή την εκ νέου δημιουργία ομάδας συνδεδεμένη τοποθεσία.

 Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

Λήψη [κέλυφος διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με το powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Καταργήστε την τοποθεσία από διαγραφή τοποθεσίες χρησιμοποιώντας το cmdlet powershell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Εάν δημιουργείτε μια συνδεδεμένη τοποθεσία ομάδας και λάβετε μια προειδοποίηση, υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το Κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήσετε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.

Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε τις σύγχρονες ομάδες με το SharePoint.

Μπορείτε να συνδέσετε τις υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [σύνδεση μια ομάδα Office 365 χρησιμοποιώντας το ineterface χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας του Office 365, θα χρειαστεί να δημιουργήσετε μια τοποθεσία ομάδας. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Δημιουργία τοποθεσίας ομάδας του SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).
