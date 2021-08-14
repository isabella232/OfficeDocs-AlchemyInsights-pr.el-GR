---
title: Υπηρεσίες μεταφοράς - Μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940056"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Υπηρεσίες μεταφοράς - Μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή

**Μετακίνηση πόρων**

Οι πόροι Azure μπορούν να μετακινηθούν σε μια άλλη συνδρομή Azure ή ομάδα πόρων στην ίδια συνδρομή χρησιμοποιώντας την πύλη Azure, το Azure PowerShell, το Azure CLI ή το REST API για να μετακινήσετε πόρους.

Για να μετακινήσετε πόρους, ανατρέξτε στα θέμα:

- [Λίστα ελέγχου πριν από τη μετακίνηση πόρων](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Υπηρεσίες που μπορούν να μετακινηθούν](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Τρόπος επικύρωσης της μετακίνησης](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Μετακίνηση καθοδήγησης για υπηρεσίες](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Για να μετακινήσετε υπάρχοντες πόρους σε άλλη ομάδα πόρων ή συνδρομή, μπορείτε να χρησιμοποιήσετε:

- [Πύλη Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Πρόγραμμα εκμάθησης: [Μετακίνηση πόρων Azure σε άλλη ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Αντιμετώπιση σφαλμάτων με τη Διαχείριση πόρων Azure**

Ανατρέξτε στα παρακάτω άρθρα για να μάθετε περισσότερα σχετικά με ορισμένα κοινά σφάλματα ανάπτυξης Azure και να λάβετε πληροφορίες για την επίλυσή τους. Εάν δεν μπορείτε να βρείτε τον κωδικό σφάλματος για το σφάλμα ανάπτυξης, ανατρέξτε στο θέμα [Εύρεση κωδικού σφάλματος.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Αντιμετώπιση σφαλμάτων ανάπτυξης](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Αντιμετώπιση προβλημάτων μετακίνησης πόρων Του Azure σε νέα ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Σημειώστε ότι εάν θέλετε να αναβαθμίσετε τη συνδρομή σας στο Azure, όπως η μετάβαση από δωρεάν σε pay-as-you-go, θα πρέπει να μετατρέψετε τη συνδρομή σας.

- Για να αναβαθμίσετε μια δωρεάν δοκιμαστική έκδοση, ανατρέξτε στο θέμα Αναβάθμιση της δωρεάν [δοκιμαστικής έκδοσης ή της συνδρομής microsoft Imagine Azure σε Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Για να αλλάξετε έναν λογαριασμό pay-as-you-go, ανατρέξτε στο θέμα Αλλαγή της συνδρομής [σας στο Azure Pay-As-You-Go σε διαφορετική προσφορά.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Για να προσθέσετε ή να συσχετίσετε μια συνδρομή Azure στον Azure Active Directory σας:**

1. Πραγματοποιήστε είσοδο και επιλέξτε τη συνδρομή που θέλετε να χρησιμοποιήσετε από [τη σελίδα "Συνδρομές" στην πύλη Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Επιλέξτε **"Αλλαγή καταλόγου".**
3. Εξετάστε τυχόν προειδοποιήσεις που εμφανίζονται και, στη συνέχεια, επιλέξτε **"Αλλαγή".**
4. Ο κατάλογος αλλάζει για τη συνδρομή και θα λάβετε ένα μήνυμα επιτυχίας.
5. Χρησιμοποιήστε την *εναλλαγή καταλόγου* για να μεταβείτε στον νέο κατάλογο. Μπορεί να χρειαστεί έως και 10 λεπτά για να εμφανίζονται σωστά τα πάντα.

**Προτεινόμενα έγγραφα**

- [Μεταβίβαση κυριότητας μιας συνδρομής Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Μετακίνηση πόρων σε νέα ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Διαχείριση πόρων με χρήση της πύλης Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
