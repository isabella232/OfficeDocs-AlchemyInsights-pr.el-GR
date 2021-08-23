---
title: Η προεπιλεγμένη Outlook ετικέτας δεν έχει εφαρμοστεί
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454755"
---
# <a name="default-outlook-label-setting-not-applied"></a>Η προεπιλεγμένη Outlook ετικέτας δεν έχει εφαρμοστεί

Εάν οι προεπιλεγμένες ρυθμίσεις ετικετών του Outlook δεν εφαρμόζονται σωστά και έχει εφαρμοστεί διαφορετική ετικέτα ή δεν έχει εφαρμοστεί ετικέτα, μπορεί να αντιμετωπίζετε ένα γνωστό πρόβλημα (MC277818) και θα πρέπει να κάνετε μία από τις παρακάτω 2 επιλογές για να επιλύσετε το πρόβλημα:

**Επιλογή 1:**

1. Μεταβείτε στο Microsoft 365 Συμμόρφωσης και > **Προστασίας πληροφοριών για**  >  **λύσεις.**
1. Επιλέξτε **"Πολιτικές ετικέτας"** και επιλέξτε την πολιτική ετικετών που πρέπει να επεξεργαστείτε ( Η ρύθμιση **του OutlookDefaultlabel** δεν έχει οριστεί σωστά στην εν λόγω πολιτική ετικέτας. Εκτελέστε **την πολιτική get-labelpolicy για** να προβάλετε αυτήν τη ρύθμιση) και, στη συνέχεια, επιλέξτε **"Επεξεργασία πολιτικής".**
1. Επιλέξτε **"Επόμενο"** μέχρι να εμφανιστεί η ρύθμιση "Εφαρμογή αυτής της προεπιλεγμένης ετικέτας σε μηνύματα ηλεκτρονικού ταχυδρομείου", η οποία είναι διαθέσιμη εάν επιλέξετε "Να απαιτείται από τους χρήστες να εφαρμόζουν μια ετικέτα στα μηνύματα ηλεκτρονικού ταχυδρομείου και τα έγγραφα των διατεταγών" στο παράθυρο διαλόγου "Ρυθμίσεις πολιτικής".   
1. Στο παράθυρο **διαλόγου "Εφαρμογή προεπιλεγμένης ετικέτας σε έγγραφα",** επιλέξτε **"Κανένα"** από την αναπτυσσόμενη λίστα.
1. Επιλέξτε **"Επόμενο"** και **"Υποβολή"** για να αποθηκεύσετε τις ρυθμίσεις ετικέτας.

**Επιλογή 2:**

Στο [Powershell του](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Κέντρου ασφάλειας και συμμόρφωσης, χρησιμοποιήστε το commandlet Set-LabelPolicy για να αλλάξετε το **OutlookDefaultlabel** σε **"Κανένα"** στο {OutlookDefaultLabel="None"}.

Εκτέλεση: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Για περισσότερες πληροφορίες σχετικά με τις προεπιλεγμένες ετικέτες Outlook, ανατρέξτε στο [θέμα Ορισμός διαφορετικής προεπιλεγμένης ετικέτας για Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)