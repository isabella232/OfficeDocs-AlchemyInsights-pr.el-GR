---
title: Μεταφορά υπηρεσιών-μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692043"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Μεταφορά υπηρεσιών-μετακίνηση όλων των υπηρεσιών RDFE σε άλλη συνδρομή

**Μετακίνηση πόρων**

Οι πόροι Azure μπορούν να μετακινηθούν είτε σε μια άλλη συνδρομή Azure είτε στην ομάδα πόρων κάτω από την ίδια συνδρομή με τη χρήση της πύλης Azure, του Azure PowerShell, του Azure CLI ή του API REST για τη μετακίνηση πόρων.

Για να μπορέσετε να μετακινήσετε πόρους, ανατρέξτε στα θέματα:

- [Λίστα ελέγχου πριν από τη μετακίνηση πόρων](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Υπηρεσίες που μπορούν να μετακινηθούν](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Πώς να επικυρώσετε την κίνηση](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Μετακίνηση οδηγιών για τις υπηρεσίες](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Για να μετακινήσετε υπάρχοντες πόρους σε μια άλλη ομάδα πόρων ή συνδρομή, μπορείτε να χρησιμοποιήσετε τα εξής:

- [Πύλη Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Πρόγραμμα εκμάθησης: [Μετακίνηση των πόρων Azure σε άλλη ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Αντιμετώπιση σφαλμάτων με τη διαχείριση πόρων του Azure**

Ανατρέξτε στα παρακάτω άρθρα για να μάθετε περισσότερα σχετικά με ορισμένα συνηθισμένα σφάλματα ανάπτυξης του Azure και να λάβετε πληροφορίες για να τα επιλύσετε. Εάν δεν μπορείτε να βρείτε τον κωδικό σφάλματος για το σφάλμα ανάπτυξης, ανατρέξτε στο θέμα [Εύρεση κωδικού σφάλματος](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Αντιμετώπιση σφαλμάτων ανάπτυξης](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Αντιμετώπιση προβλημάτων μετακίνησης πόρων Azure σε νέα ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Λάβετε υπόψη ότι, εάν θέλετε να αναβαθμίσετε τη συνδρομή σας στο Azure, όπως η μετάβαση από τη δυνατότητα "δωρεάν" σε "Pay-as-you-Go", θα χρειαστεί να μετατρέψετε τη συνδρομή σας.

- Για να αναβαθμίσετε μια δωρεάν δοκιμαστική έκδοση, ανατρέξτε στο θέμα [αναβάθμιση της δωρεάν δοκιμαστικής έκδοσης ή της συνδρομής σας στο Microsoft φανταστούμε ότι θα πληρώσετε-as-you-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Για να αλλάξετε ένα λογαριασμό Pay-as-you-Go, ανατρέξτε [στο θέμα Αλλαγή της συνδρομής σας με τη συνδρομή Azure Pay-as-you-Go σε διαφορετική προσφορά](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Για να προσθέσετε ή να συσχετίσετε μια συνδρομή Azure στο μισθωτή του Azure Active Directory:**

1. Πραγματοποιήστε είσοδο και επιλέξτε τη συνδρομή που θέλετε να χρησιμοποιήσετε από τη [σελίδα "συνδρομές" στην πύλη Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Επιλέξτε **αλλαγή καταλόγου**.
3. Εξετάστε τυχόν προειδοποιήσεις που εμφανίζονται και, στη συνέχεια, επιλέξτε **Αλλαγή**.
4. Ο κατάλογος έχει αλλάξει για τη συνδρομή και θα λάβετε ένα μήνυμα επιτυχίας.
5. Χρησιμοποιήστε την εναλλαγή *καταλόγων* για να μεταβείτε στον νέο σας κατάλογο. Μπορεί να χρειαστούν έως και 10 λεπτά για να εμφανιστούν όλα τα στοιχεία σωστά.

**Προτεινόμενα έγγραφα**

- [Μεταφορά της κυριότητας μιας συνδρομής Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Μετακίνηση πόρων σε νέα ομάδα πόρων ή συνδρομή](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Διαχείριση πόρων με χρήση της πύλης Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
