---
title: Εύρεση εφαρμογών που λείπουν στο Blade εγγραφής εφαρμογών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404693"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Εύρεση εφαρμογών που λείπουν στο Blade εγγραφής εφαρμογών

1. Δεν είναι δυνατή η εύρεση εφαρμογών στην πύλη καταχώρησης εφαρμογών.

    Εάν μια εφαρμογή είναι μια εφαρμογή πολλών μισθωτών και έχει καταχωρηθεί σε άλλο μισθωτή, δεν θα εμφανίζεται στην περιοχή "Εγγραφή εφαρμογής". Ωστόσο, μπορεί να το βρείτε στην περιοχή Enterprise Applications blade αφού αποκτήσετε πρόσβαση (μετά τη συγκατάθεσή σας) και η κύρια υπηρεσία έχει δημιουργηθεί στο μισθωτή σας. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εφαρμογές και & υπηρεσίες στο Azure AD - Πλατφόρμα ταυτότητας της Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Δεν είναι δυνατή η προβολή εφαρμογών στο Δίσκο εγγραφής εφαρμογών, παρόλο που είστε διαχειριστής.

    Βεβαιωθείτε ότι είστε στον σωστό κατάλογο στην πύλη Azure.
3. Η εφαρμογή μου δεν εμφανίζεται στην περιοχή Enterprise Applications blade, αλλά εμφανίζεται όταν κάνω ερώτημα στην εντολή PowerShell.

    Ορισμένες φορές, αφού διαγράψετε την εφαρμογή από την πύλη Azure, δεν εμφανίζεται στην πύλη, αλλά ενδέχεται να μην έχει διαγραφεί πλήρως. Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:
    - Μπορείτε να ανακτήσετε τη λίστα των εφαρμογών που έχουν διαγραφεί προηγουμένως και να δείτε εάν η εφαρμογή εμφανίζεται στη λίστα χρησιμοποιώντας την εντολή Powershell: **Get-AzureADDeletedApplication.** Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Εάν θέλετε να καταργήσετε εντελώς την εφαρμογή, μπορείτε να δοκιμάσετε τα εξής στο PowerShell: **Remove-AzureADApplication -ObjectId.** Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Κατάργηση-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Εναλλακτικά, μπορείτε να δοκιμάσετε να επαναφέρετε τη διαγραμμένη εφαρμογή χρησιμοποιώντας την ακόλουθη εντολή powershell: **Επαναφορά AzureADDeletedApplication -ObjectId.** Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Επαναφορά-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Δεν μπορώ να βρω τη λίστα όλων των προεγκατεστημενών εταιρικών εφαρμογών στο νέο μου μισθωτή Azure.

    Δεν υπάρχουν προεγκατεστημενές εταιρικές εφαρμογές στο Azure AD από προεπιλογή. Πρέπει να την προσθέσετε με μη αυτόματο τρόπο από την επιλογή "Νέα εφαρμογή", περιηγείστε την από τη συλλογή Azure AD ή προσθέστε μια εφαρμογή που δεν είναι συλλογή. Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Γρήγορη εκκίνηση: Προσθήκη εφαρμογής στο μισθωτή Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Εάν είστε καθολικός διαχειριστής, μπορείτε εύκολα να αποκτήσετε πρόσβαση στις εφαρμογές σας χρησιμοποιώντας [την Εκκίνηση εφαρμογών του Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Δεν είναι δυνατή η εύρεση των εφαρμογών μου από την πύλη "Οι εφαρμογές μου".

    Βεβαιωθείτε ότι οι εφαρμογές δεν είναι κρυφές στη σελίδα συλλογής "Οι εφαρμογές μου". Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Συλλογές (προεπισκόπηση) στην πύλη "Οι εφαρμογές μου" - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Για να ξεκινήσετε εφαρμογές από την πύλη "Οι εφαρμογές μου", ανατρέξτε στο [θέμα "Εντοπισμός & χρήση εφαρμογών στην πύλη "Οι εφαρμογές μου" - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Η εφαρμογή Office 365 Mover δεν εμφανίζεται στο Blade για μεγάλες εφαρμογές μετά την εγκατάσταση.

    Η εφαρμογή "Office 365 Mover" είναι μια εφαρμογή πολλαπλών εφαρμογών που δεν χρειάζεται να προστεθεί στο AAD χρησιμοποιώντας την ενότητα "Εφαρμογές συλλογής" στην περιοχή "Εγγραφή εφαρμογής για μεγάλες επιχειρήσεις". Για να αποκτήσετε πρόσβαση στην εφαρμογή Office 365 Mover, απλώς πραγματοποιήστε είσοδο στην εφαρμογή και θα ζητήσει τη συγκατάθεση του χρήστη για τα δικαιώματα. Όταν ο χρήστης παρέχει τη συγκατάθεση, αυτή η εφαρμογή θα προστεθεί αυτόματα στο μισθωτή με το αναγνωριστικό ηλεκτρονικού ταχυδρομείου που έχετε συνδεθεί.

    Μετά την είσοδο στην εφαρμογή, θα πρέπει να μπορείτε να βρείτε την καταχώρηση αυτής της εφαρμογής κάτω από τη λάμα των εταιρικών εφαρμογών στο AAD. Πρέπει να αναζητήσετε αυτή την εφαρμογή πληκτρολογώντας το πλήρες όνομα, π.χ., "Office 365 Mover" ή απλώς κάντε αναζήτηση στο "office" και θα πρέπει να καταχωρήσει την εφαρμογή. Για να μάθετε περισσότερα, ανατρέξτε στο [θέμα Του Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)που αναφέρει ότι είναι ήδη εγκατεστημένο, αλλά δεν αναφέρεται στη συλλογή εταιρικών εφαρμογών.
8. Γρήγορη εκκίνηση: Η προβολή της λίστας των εφαρμογών που χρησιμοποιούν το μισθωτή [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) για τη διαχείριση ταυτότητας σάς δείχνει πώς μπορείτε να προβάλετε τις εφαρμογές, γνωστές και ως εφαρμογές, που έχουν ήδη ρυθμιστεί ώστε να χρησιμοποιούν το μισθωτή Azure AD ως υπηρεσία παροχής ταυτότητας (IdP).
9. [Αντιμετώπιση συνηθισμένων προβλημάτων με την προσθήκη ή την](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) κατάργηση μιας εφαρμογής στο Azure Active Directory σάς βοηθά να κατανοήσετε τα συνήθη προβλήματα που αντιμετωπίζουν οι χρήστες κατά την προβολή εφαρμογών στο Azure Active Directory.
