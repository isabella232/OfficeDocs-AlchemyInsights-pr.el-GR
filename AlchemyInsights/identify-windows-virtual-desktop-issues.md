---
title: Προσδιορισμός προβλημάτων εικονικής επιφάνειας εργασίας των Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595629"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Προσδιορισμός προβλημάτων εικονικής επιφάνειας εργασίας των Windows

Τα Διαγνωστικά εικονικής επιφάνειας εργασίας των Windows χρησιμοποιούν μόνο ένα cmdlet του PowerShell, αλλά περιέχουν πολλές προαιρετικές παραμέτρους για να σας βοηθήσουν να περιορίσετε και να απομονώσετε προβλήματα. Για να ξεκινήσετε: 

1. Κάντε λήψη και εισαγωγή της λειτουργικής μονάδας PowerShell εικονικής επιφάνειας εργασίας των Windows. Για λεπτομέρειες, [ανατρέξτε στα Cmdlet εικονικής επιφάνειας εργασίας των Windows για το Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Εκτελέστε το ακόλουθο cmdlet για να εισέλθετε στο λογαριασμό σας:
    
    Παράδειγμα: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**ΣΗΜΕΙΩΣΗ:** Όλα τα ερωτήματα που χρησιμοποιούν το PowerShell πρέπει να περιλαμβάνουν τις παραμέτρους -Όνομα χρήστη ή -ActivityID. Για δυνατότητες παρακολούθησης, ανατρέξτε στο θέμα "Χρήση [ανάλυσης καταγραφής" για τη δυνατότητα διαγνωστικών.](https://go.microsoft.com/fwlink/?linkid=2126847)

Για να φιλτράρετε τις διαγνωστικές δραστηριότητες κατά χρήστη, εκτελέστε το ακόλουθο cmdlet:

Παράδειγμα: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Υπάρχει μια λίστα φίλτρων που μπορείτε να εκτελέσετε για τη διάγνωση προβλημάτων. Για να μάθετε περισσότερα σχετικά με τη διάγνωση προβλημάτων, ανατρέξτε στο θέμα [Αναγνώριση και διάγνωση ζητημάτων εικονικής επιφάνειας εργασίας των Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Για να μάθετε περισσότερα σχετικά με τα συνηθισμένα σφάλματα, ανατρέξτε στο θέμα [Κοινά σφάλματα senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
