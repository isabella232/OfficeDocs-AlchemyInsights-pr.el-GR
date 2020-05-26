---
title: 'Σαρωτής AIP: εγκατάσταση και διαμόρφωση'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357664"
---
# <a name="aip-scanner-installation-and-configuration"></a>Σαρωτής AIP: εγκατάσταση και διαμόρφωση

**Για να εγκαταστήσετε το σαρωτή AIP, ακολουθήστε τις προτεινόμενες οδηγίες:**

1. Εάν κάνετε αναβάθμιση και δεν εκτελείτε μια καθαρή εγκατάσταση, βεβαιωθείτε ότι έχετε ακολουθήσει τις οδηγίες για [την αναβάθμιση του σαρωτή προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) και για ενοποιημένη επισήμανση του υπολογιστή-πελάτη, [ανατρέξτε στο θέμα αναβάθμιση του σαρωτή προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Βεβαιωθείτε ότι συμμορφώνεστε με [όλες τις απαιτήσεις ρυθμίσεων τείχους προστασίας και υποδομής δικτύου](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Βεβαιωθείτε ότι [οι πολιτικές](https://docs.microsoft.com/azure/information-protection/configure-policy) σας έχουν οριστεί σε αυτόματη επισήμανση ή έχουν μια προεπιλεγμένη ετικέτα στην πολιτική.
4. Βεβαιωθείτε ότι ο σχετικός τύπος αρχείου έχει ρυθμιστεί για ετικέτα/προστασία, όπως περιγράφεται στο [φάκελο "Τύποι αρχείων" που υποστηρίζονται από το πρόγραμμα-πελάτη Προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Επιπλέον, εάν θέλετε να αλλάξετε την προεπιλεγμένη συμπεριφορά, ακολουθήστε τις παρακάτω οδηγίες: [Αλλαγή του προεπιλεγμένου επιπέδου προστασίας των αρχείων](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Βεβαιωθείτε ότι ο λογαριασμός χρήστη που έχει ρυθμιστεί για την εκτέλεση της υπηρεσίας σαρωτή έχει δικαιώματα πρόσβασης σε όλα τα ρυθμισμένα αποθετήρια.
6. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, εξαγάγετε τα αρχεία καταγραφής σαρωτή και προσθέστε τα στο δελτίο υποστήριξης.

**Εξαγωγή αρχείων καταγραφής σαρωτή προστασίας πληροφοριών Azure**

1. Μεταβείτε στα %localappdata%\Microsoft\MSIP κάτω από το περιβάλλον χρήστη που εκτελεί την υπηρεσία σαρωτή.
2. Φερμουάρ όλα τα περιεχόμενα κάτω από το φάκελο MSIP.
3. Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή τοποθεσίας σας και επισυνάψτε τα στο αίτημα εξυπηρέτησης.
4. Μπορείτε επίσης να χρησιμοποιήσετε [εξαγωγή-AIPLogs -Εκ μέρους του](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Για περισσότερες πληροφορίες, ανατρέξτε**στα θέματα :
- [Ανάπτυξη του σαρωτή προστασίας πληροφοριών Azure για αυτόματη ταξινόμηση και προστασία αρχείων](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Καθορισμός και χρήση της παραμέτρου Διακριτικού για set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Εκτέλεση κύκλου εντοπισμού και προβολή αναφορών για το σαρωτή](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Απαιτήσεις για την προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Λήψη προγράμματος-πελάτη προστασίας πληροφοριών Azure](https://www.microsoft.com/download/details.aspx?id=53018)
