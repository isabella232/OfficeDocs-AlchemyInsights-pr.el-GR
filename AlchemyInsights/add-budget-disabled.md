---
title: Γιατί το κουμπί "Προσθήκη προϋπολογισμού" είναι απενεργοποιημένο για εμένα;
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954671"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Γιατί το κουμπί "Προσθήκη προϋπολογισμού" είναι απενεργοποιημένο για εμένα;

Για να δημιουργήσετε έναν προϋπολογισμό, χρειάζεστε ένα από τα ακόλουθα δικαιώματα:

- Ομάδα διαχείρισης, συνδρομές, εύρος ομάδας πόρων
- Συνεργάτης διαχείρισης κόστους
- Κάτοχος
- Συνεργάτης
- Μόνο για εταιρικούς πελάτες: Εγγραφή, Τμήμα, Εύρος λογαριασμού
- Διαχειριστής εγγραφής (ορισμός προϋπολογισμού στο εύρος εγγραφής)
- Διαχειριστής τμήματος (ορισμός προϋπολογισμού στο πεδίο εφαρμογής του τμήματος)
- Κάτοχος λογαριασμού (ορισμός προϋπολογισμού στο πεδίο εφαρμογής λογαριασμού)
- Σύγχρονη σύμβαση πελάτη μόνο: Λογαριασμός χρέωσης, Προφίλ χρέωσης, Εύρος ενοτήτων τιμολογίου
- Δημιουργός συνδρομής Azure

**Δημιούργησα έναν προϋπολογισμό όταν το κόστος μου για τον τρέχοντα μήνα ήταν ήδη υπερ-προϋπολογισμός. Γιατί δεν λαμβάνω μια ειδοποίηση;**  
Εάν έχετε ήδη υπερβεί ένα δεδομένο όριο κόστους όταν δημιουργείτε έναν προϋπολογισμό που δεν θα σας ειδοποιήσει. Μόλις ξεκινήσει ένας νέος κύκλος, εάν παραβιάσετε το όριο, η ειδοποίηση θα ξεκινήσει.

**Πότε θα πρέπει να αναμένω να λαμβάνω μια ειδοποίηση μετά την υπέρβαση ενός από τα καθορισμένα όρια ειδοποιήσεων προϋπολογισμού;**  
Οι προϋπολογισμοί αξιολογούνται κάθε 4 ώρες. Χρειάζονται τουλάχιστον 8 ώρες για να φτάσουν τα δεδομένα χρήσης στο σύστημα προϋπολογισμών. Με αυτό το δεδομένο, οι ειδοποιήσεις μπορεί να διαρκέσει έως και 12 ώρες για να γίνει η πυρόσβεση αφού υπερβείτε ένα όριο.

**Γιατί το κουμπί "Ημερομηνία έναρξης" είναι απενεργοποιημένο όταν επιλέγω μια περίοδο επαναφοράς μήνα ή μήνα χρέωσης;**  
Οι προϋπολογισμοί ευθυγραμμίζονται με τον τρέχοντα ημερολογιακό μήνα ή την τρέχουσα περίοδο χρέωσης (στην περίπτωση που είναι επιλεγμένος ο μήνας χρέωσης). Επομένως, η προ-συμπλήρωση αυτής της τιμής για εσάς.

**Γιατί δεν βλέπω ένα γράφημα του κόστους μου στην εμπειρία δημιουργίας προϋπολογισμού;**  
Χρειαζόμαστε τουλάχιστον 2 μήνες δεδομένων κόστους για να μπορούμε να κάνουμε ένα γράφημα για να σας βοηθήσουμε με τη δημιουργία του προϋπολογισμού.

**Γιατί δεν μπορώ να ρυθμίσω έναν προϋπολογισμό σε σχέση με μια συνδρομή που μόλις δημιούργησα;**  
Μετά τη δημιουργία μιας συνδρομής, τα δεδομένα χρειάζονται 24-48 ώρες για να επεξεργαστούν πριν από τη ρύθμιση ενός προϋπολογισμού σε σχέση με αυτό.

**Πόροι API προϋπολογισμού**

- [API προϋπολογισμών v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Παρέχει λειτουργίες για τη δημιουργία και την ενημέρωση προϋπολογισμών. Χρησιμοποιώντας το API προϋπολογισμών, μπορείτε να ορίσετε ένα όριο προϋπολογισμού και να ρυθμίσετε πολλές ειδοποιήσεις ώστε να σβήνουν καθώς πλησιάζετε αυτό το όριο. Οι ειδοποιήσεις μπορούν να ενεργοποιήσουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου ή μια ομάδα ενεργειών Azure για την εκτέλεση αυτοματοποίησης. Σημείωση: Το φιλτράρισμα για αυτό το API δεν ευθυγραμμίζεται με το φιλτράρισμα /τις διαστάσεις api ερωτήματος.
- [Api προϋπολογισμών v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Δημιουργία προϋπολογισμών με δυνατότητες φιλτραρίσματος μεγαλύτερου κόστους από ό,τι v1. Το φιλτράρισμα στοιχίζεται στη σύμβαση που χρησιμοποιείται στα API ερωτήματος και διαστάσεων. Αυτό είναι το προτεινόμενο API προϋπολογισμών για χρήση της μετακίνησης προς τα εμπρός.
- [Διαστάσεις:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Παρέχει λειτουργίες για να λάβετε υποστηριζόμενες διαστάσεις για τη χρήση σας κάτω από μια ποικιλία εύρους. Χρησιμοποιώντας το API "Διαστάσεις", μπορείτε να ανακτήσετε μια λίστα διαστάσεων που μπορούν να χρησιμοποιηθούν ως είσοδοι για τη δημιουργία ερωτημάτων με το API ερωτήματος.
- [Ερώτημα:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Παρέχει λειτουργίες για τη λήψη συγκεντρωτικών δεδομένων κόστους και χρήσης με βάση το ερώτημα που θα δώσετε. Χρησιμοποιώντας το API ερωτήματος, μπορείτε να καθορίσετε το επιθυμητό φιλτράρισμα, ταξινόμηση και ομαδοποίηση σε όλες τις διαθέσιμες διαστάσεις (στις οποίες έχετε πρόσβαση από το API διαστάσεων).

**Προβλεπόμενο κόστος**

**Γιατί δεν βλέπω προβλέψεις για το κόστος μου στην Ανάλυση κόστους;**  
Υπάρχουν πολλοί λόγοι για τους οποίους η προβολή πρόβλεψης μπορεί να λείπει για εσάς στην Ανάλυση κόστους, ορισμένοι από αυτούς είναι οι εξής:

1. Εάν τα δεδομένα κόστους είναι λιγότερα από 10 ημέρες, το γράφημα πρόβλεψης δεν θα φορτωθεί. Το μοντέλο απαιτεί τουλάχιστον 10 ημέρες πρόσφατων δεδομένων κόστους για ακριβείς προβολές
2. Εάν έχετε επιλέξει ιστορικές ημερομηνίες, τότε το γράφημα πρόβλεψης δεν θα είναι ορατό. Επιλέξτε ένα εύρος ημερομηνιών με μελλοντικές ημερομηνίες για να εμφανιστεί το γράφημα πρόβλεψης
3. Εάν ο λογαριασμός σας έχει πολλά νομίσματα, το γράφημα πρόβλεψης θα προβλέπει μόνο το κόστος για το "Όλο το κόστος σε δολάρια ΗΠΑ"

**Γιατί η πρόβλεψη δεν αλλάζει όταν κάνω αλλαγές στους πόρους μου;**  
Το μοντέλο πρόβλεψης απαιτεί μερικές ημέρες για να ληφθούν υπόψη οι αλλαγές στο λογαριασμό και δεν κάνει άμεσες προβολές με βάση την αλλαγή των πόρων  
Για μεγαλύτερα βήματα αύξησης ή μείωσης των πόρων, το μοντέλο θα χρειαστεί λίγο περισσότερο χρόνο για να προσαρμοστεί σε αυτές τις αλλαγές ώστε να ληφθούν υπόψη οι ανωμαλιές

**Γιατί αυξάνεται η πρόβειά μου μετά την κράτηση ή την αγορά του Marketplace;**  
Το μοντέλο πρόβλεψης λαμβάνει υπόψη το "Πραγματικό κόστος" και δεν λαμβάνει υπόψη τη χρήση και την αγορά ξεχωριστά. Για μια αγορά μίας φοράς, το μοντέλο θα μειώσει τις προβολές μετά από 10 ημέρες για να ληφθεί υπόψη η αιφνίδια αύξηση του κόστους

**Θέλω να δω προβλέψεις για μία μόνο διάσταση (π.χ. Μετρητής)**  
Η πρόβλεψη υποστηρίζει επί του παρόντος προβολές συνολικού κόστους και όχι μεμονωμένους μετρητές. Επομένως, όταν "Ομαδοποιηθηκε κατά" μια διάσταση, οι προβολές θα είναι για το σύνολο όλων των στοιχείων της διάστασης

**Προτεινόμενα έγγραφα**

- [Τι είναι η Διαχείριση κόστους Azure;](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Βέλτιστες πρακτικές διαχείρισης κόστους Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ανάλυση του κόστους και των δαπανών σας](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Εξερεύνηση και ανάλυση κόστους με ανάλυση κόστους](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Διαχείριση κόστους Azure: Τιμολόγηση](https://azure.microsoft.com/services/cost-management/#pricing)
- [Εξέταση κόστους στην ανάλυση κόστους](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Βίντεο εκμάθησης: Δημιουργία προϋπολογισμού στην πύλη Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Προαπαιτούμενα για την προβολή και την προσαρμογή προϋπολογισμών](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Δημιουργία και διαχείριση προϋπολογισμών](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Ρύθμιση παραμέτρων αυτοματοποίησης με το Azure Action Groups και το API προϋπολογισμών](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Χρήση ειδοποιήσεων κόστους για την παρακολούθηση της χρήσης και των δαπανών](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Βέλτιστες πρακτικές διαχείρισης κόστους](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Βίντεο εκμάθησης**

- [Δημιουργία προϋπολογισμού στην πύλη Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Διαχείριση κόστους με το API προϋπολογισμών και τις ομάδες ενεργειών](https://go.microsoft.com/fwlink/?linkid=2147038)