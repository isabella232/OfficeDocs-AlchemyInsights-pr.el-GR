---
title: 'Σαρωτής AIP: εγκατάσταση και ρύθμιση παραμέτρων'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934257"
---
# <a name="aip-scanner-installation-and-configuration"></a>Σαρωτής AIP: εγκατάσταση και ρύθμιση παραμέτρων

**Για να εγκαταστήσετε το σαρωτή AIP, ακολουθήστε τις προτεινόμενες οδηγίες:**

1. Εάν κάνετε αναβάθμιση και δεν εκτελείτε καθαρή εγκατάσταση, βεβαιωθείτε ότι έχετε ακολουθήσει τις οδηγίες για την αναβάθμιση του [σαρωτή προστασίας](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) πληροφοριών Azure και για το ενοποιημένο πρόγραμμα-πελάτη σήμανσης, ανατρέξτε στο θέμα αναβάθμιση του σαρωτή Προστασίας [πληροφοριών Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Βεβαιωθείτε ότι συμμορφώνεστε με όλα τα [Τείχη προστασίας και τις απαιτήσεις ρυθμίσεων υποδομής δικτύου.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Βεβαιωθείτε ότι οι [πολιτικές σας έχουν](https://docs.microsoft.com/azure/information-protection/configure-policy) οριστεί σε αυτόματη σήμανση ή ότι έχουν μια προεπιλεγμένη ετικέτα στην πολιτική.
4. Βεβαιωθείτε ότι ο σχετικός τύπος αρχείου έχει ρυθμιστεί για ετικέτα/προστασία, όπως περιγράφεται στους τύπους [αρχείων που υποστηρίζονται από το πρόγραμμα-πελάτη Προστασίας πληροφοριών Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Επιπλέον, εάν θέλετε να αλλάξετε την προεπιλεγμένη συμπεριφορά, ακολουθήστε τις παρακάτω οδηγίες: [Αλλαγή του προεπιλεγμένου επιπέδου προστασίας αρχείων.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Βεβαιωθείτε ότι ο λογαριασμός χρήστη που έχει ρυθμιστεί για την εκτέλεση της υπηρεσίας σαρωτή έχει δικαιώματα πρόσβασης σε όλα τα ρυθμισμένα αποθετήρια.
6. Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, εξαγάγετε τα αρχεία καταγραφής του σαρωτή και προσθέστε τα στο δελτίο υποστήριξης.

**Εξαγωγή αρχείων καταγραφής του Σαρωτή προστασίας πληροφοριών Azure**

1. Μεταβείτε στο %localappdata%\Microsoft\MSIP κάτω από το περιβάλλον χρήστη που εκτελεί την υπηρεσία σαρωτή.
2. Συμπίεση όλων των περιεχομένων κάτω από το φάκελο MSIP.
3. Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή θέσης σας και επισυνάψτε τα στην αίτηση εξυπηρέτησης.
4. Μπορείτε επίσης να χρησιμοποιήσετε [το Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Για πρόσθετες πληροφορίες, ανατρέξτε στο θέμα:**
- [Ανάπτυξη του σαρωτή προστασίας πληροφοριών Azure για την αυτόματη ταξινόμηση και προστασία αρχείων](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Καθορισμός και χρήση της παραμέτρου Διακριτικού για το Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Εκτέλεση κύκλου εντοπισμού και προβολή αναφορών για το σαρωτή](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Αναθεώρηση τεκμηρίωσης της Προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Απαιτήσεις για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Λήψη προγράμματος-πελάτη Προστασίας πληροφοριών Azure](https://www.microsoft.com/download/details.aspx?id=53018)
