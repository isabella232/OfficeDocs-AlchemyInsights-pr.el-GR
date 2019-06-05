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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719482"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Δημιουργία ομάδας συνδεδεμένη τοποθεσία στο SharePoint Online

<p><strong>Υπάρχουν μερικά κοινά θέματα που προέκυψαν κατά τη δημιουργία ή την εκ νέου δημιουργία ομάδας συνδεδεμένη τοποθεσία.&nbsp;</strong></p>  <p>1.Εάν έχετε διαγράψει μια ομάδα και τη συνδεδεμένη τοποθεσία και θέλετε να δημιουργήσετε μια άλλη τοποθεσία με την ίδια διεύθυνση URL, θα πρέπει να καταργήσετε οριστικά την προηγούμενη τοποθεσία.</p>  <ul>  <li>Άμεση λήψη του <a title="κέλυφος διαχείρισης SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Κέλυφος διαχείρισης SPO</a> - για περισσότερες πληροφορίες σχετικά με γρήγορα αποτελέσματα με το powershell, ανατρέξτε στην ενότητα <a title="γρήγορα αποτελέσματα με την ηλεκτρονική κέλυφος διαχείρισης του SharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Γρήγορα αποτελέσματα με το SharePoint Online κέλυφος διαχείρισης</a>. <br /><br /></li>  <li>Καταργήστε την τοποθεσία από διαγραφή τοποθεσίες χρησιμοποιώντας το <a title="SPODeletedSite κατάργηση" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Κατάργηση SPODeletedSite</a> το cmdlet powershell.</li>  </ul>  <p>Εάν δημιουργείτε μια συνδεδεμένη τοποθεσία ομάδας και λάβετε μια προειδοποίηση <strong>'υπάρχει μια άλλη ομάδα με το ίδιο ψευδώνυμο ήδη'</strong>, ελέγξτε τις υπάρχουσες ομάδες από το <a title="Office 365 από το Κέντρο διαχείρισης" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 από το Κέντρο διαχείρισης</a>. Για να επιλύσετε αυτό το ζήτημα, διαγράψτε την υπάρχουσα ομάδα, εάν δεν είναι πλέον απαραίτητη ή δημιουργήσετε την τοποθεσία με διαφορετικό ψευδώνυμο που έχει αντιστοιχιστεί.&nbsp;</p>  <p><strong>Υπάρχουν διάφοροι τρόποι για να δημιουργήσετε και να χρησιμοποιήσετε τις σύγχρονες ομάδες με το SharePoint.&nbsp;</strong></p>  <ol>  <li>Μπορείτε να συνδέσετε τις υπάρχουσες τοποθεσίες σε μια ομάδα του Office 365. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα <a title="σύνδεση μια ομάδα Office 365 χρησιμοποιώντας το ineterface χρήστη του SharePoint" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Συνδέστε μια ομάδα Office 365 χρησιμοποιώντας το ineterface χρήστη του SharePoint</a>.</li>  <li>Για να δημιουργήσετε μια συνδεδεμένη τοποθεσία ομάδας του Office 365, θα χρειαστεί να δημιουργήσετε μια τοποθεσία ομάδας. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα <a title="Δημιουργήστε μια τοποθεσία ομάδας στο SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Δημιουργήστε μια τοποθεσία ομάδας του SharePoint.</a></li>  </ol>

