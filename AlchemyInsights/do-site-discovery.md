---
title: Εντοπισμός τοποθεσίας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030758"
---
# <a name="do-site-discovery"></a>Εντοπισμός τοποθεσίας

Εάν ο οργανισμός σας εξακολουθεί να χρησιμοποιεί εφαρμογές Web παλαιού τύπου και σχεδιάζει να χρησιμοποιήσει τη λειτουργία Internet Explorer (που κάνουν οι περισσότεροι πελάτες), τότε θα πρέπει να κάνετε κάποιο πρόσθετο εντοπισμό τοποθεσίας.

**Έχετε ήδη αναπτύξει μια παλαιότερη έκδοση του Microsoft Edge**

Εάν έχετε ήδη ρυθμίσει τις παραμέτρους της λίστας εταιρικών τοποθεσιών ώστε να λειτουργεί για την προηγούμενη έκδοση του Microsoft Edge, τότε ο εντοπισμός της τοποθεσίας σας έχει σχεδόν τελειώσει. Το μόνο πράγμα που ίσως χρειαστεί να κάνετε είναι να προσθέσετε ουδέτετες τοποθεσίες.

Οι ουδέτερες τοποθεσίες είναι συνήθως τοποθεσίες που παρέχουν μία σύνδεση (SSO). Εάν μεταβείτε σε μια ουδέτερη τοποθεσία από Microsoft Edge, τότε θέλετε να παραμείνετε σε μια Microsoft Edge έλεγχο ταυτότητας. Εάν μεταβείτε σε μια ουδέτερη τοποθεσία σε λειτουργία Internet Explorer, τότε θέλετε να παραμείνετε σε λειτουργία Internet Explorer για έλεγχο ταυτότητας.

Προσδιορίστε τυχόν SSO ή άλλες ουδέτερες τοποθεσίες που χρησιμοποιείτε και προσθέστε τις στη λίστα εταιρικών τοποθεσιών σας.

**Ο Internet Explorer είναι το προεπιλεγμένο πρόγραμμα περιήγησης**

Εάν χρησιμοποιείτε μόνο τον Internet Explorer τώρα, ενδέχεται να μην γνωρίζετε ποιες τοποθεσίες έχουν αναβαθμιστεί σε σύγχρονα πρότυπα Web και ποιες εξακολουθούν να απαιτούν internet Explorer. Θα πρέπει να βρείτε και να προσθέσετε αυτές τις τοποθεσίες στη λίστα εταιρικών τοποθεσιών, ώστε να μπορείτε να χρησιμοποιήσετε τη λειτουργία Internet Explorer μόνο για αυτές τις τοποθεσίες.

> [!NOTE]
> [Ο εντοπισμός τοποθεσίας για](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) μεγάλες επιχειρήσεις ανακαλύπτει τοποθεσίες που ενδέχεται να χρειάζονται λειτουργία Internet Explorer. Μπορεί να συλλέγει δεδομένα σε υπολογιστές που Windows Internet Explorer 8 internet Explorer 11 σε Windows 10, Windows 8.1 ή Windows 7.

**Ανάλυση των δεδομένων**

Αφού συλλέξετε δεδομένα τοποθεσίας, συνιστάται η ακόλουθη διαδικασία τεσσάρων βημάτων για την ανάλυση των δεδομένων:
1. Ταξινομήστε τα δεδομένα κατά τομέα και, στη συνέχεια, κατά διεύθυνση URL.
2. Ορίστε τα όρια μιας εφαρμογής για ρύθμιση παραμέτρων για τη λειτουργία Internet Explorer. Θέλετε να συμπεριλάβετε όλες τις τοποθεσίες και τα στοιχεία ελέγχου Web που ορίζουν την εφαρμογή, αλλά δεν θέλετε να συμπεριλάβετε επιπλέον τοποθεσίες και στοιχεία ελέγχου. Ορισμένες τοποθεσίες μπορεί να είναι τόσο απλές *https://contoso.com/app1* όσο ενώ άλλες μπορεί να απαιτούν να ορίσετε πολλές τοποθεσίες και σελίδες.
3. Ελέγξτε την εφαρμογή για να βεβαιωθείτε ότι δεν λειτουργεί εγγενώς. Πολλές τοποθεσίες θα προσφέρουν σύγχρονο περιεχόμενο όταν εντοπίζουν ένα σύγχρονο πρόγραμμα περιήγησης και προσφέρουν περιεχόμενο παλαιού τύπου μόνο όταν εντοπίζουν τον Internet Explorer.
4. Προσθέστε την εφαρμογή στη λίστα εταιρικών τοποθεσιών, εάν αποτύχει ο έλεγχος.

> [!NOTE]
> Ως βέλτιστη πρακτική, ομαδοποιήσετε όλες τις τοποθεσίες που αποτελούν μια εφαρμογή. Με αυτόν τον τρόπο, όταν αναβαθμίζετε μια εφαρμογή, είναι πιο εύκολο να καταργήσετε ολόκληρη την τοποθεσία από τη λειτουργία Internet Explorer και να αρχίσετε να χρησιμοποιείτε ένα σύγχρονο πρόγραμμα περιήγησης για αυτήν την εφαρμογή.

Όταν τελειώσετε με τον εντοπισμό τοποθεσίας και αναλύσετε τα δεδομένα, είστε έτοιμοι να αρχίσετε να ψάχνετε τη στρατηγική του καναλιού σας.

