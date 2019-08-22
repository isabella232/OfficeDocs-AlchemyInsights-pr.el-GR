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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507847"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Ζητήματα κατά τη δημιουργία ή την ομάδα συνδεδεμένες τοποθεσίες SharePoint Online

Υπάρχουν μερικά κοινά θέματα που προέκυψαν κατά τη δημιουργία ή την εκ νέου δημιουργία ομάδας συνδεδεμένη τοποθεσία.

 Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.

Λήψη [κέλυφος διαχείρισης SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με το powershell, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Καταργήστε την τοποθεσία από διαγραφή τοποθεσίες χρησιμοποιώντας το cmdlet powershell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Εάν δημιουργείτε μια συνδεδεμένη τοποθεσία ομάδας και λάβετε μια προειδοποίηση, υπάρχει ήδη μια άλλη ομάδα με το ίδιο ψευδώνυμο, ελέγξτε τις υπάρχουσες ομάδες από το [Office 365 από το Κέντρο διαχείρισης](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήσετε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.

Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε τις σύγχρονες ομάδες με το SharePoint.

Μπορείτε να συνδέσετε τις υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [σύνδεση μια ομάδα Office 365 χρησιμοποιώντας το ineterface χρήστη του SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας του Office 365, θα χρειαστεί να δημιουργήσετε μια τοποθεσία ομάδας. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Δημιουργία τοποθεσίας ομάδας του SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

