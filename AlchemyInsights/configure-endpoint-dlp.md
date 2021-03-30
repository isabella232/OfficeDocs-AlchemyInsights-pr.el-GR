---
title: Ρύθμιση παραμέτρων DLP τελικών σημείων
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402423"
---
# <a name="configure-endpoint-dlp"></a>Ρύθμιση παραμέτρων DLP τελικών σημείων

Τα DLP τελικών σημείων της Microsoft σάς επιτρέπουν να επεκτείνετε τη δυνατότητα προστασίας και παρακολούθησης DLP στις ευαίσθητες πληροφορίες σε συσκευές Windows 10. Αφού οι συσκευές εγγραφούν στη διαχείριση συσκευών, μπορείτε να δημιουργήσετε πολιτικές DLP για την επιβολή ασφαλιστικών ενεργειών σε στοιχεία. Η "Εξερεύνηση δραστηριότητας" μπορεί να χρησιμοποιηθεί για την παρακολούθηση της δραστηριότητας για ευαίσθητα στοιχεία. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών στη διαχείριση συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Για να ξεκινήσετε με τα DLP τελικών σημείων:

- Βεβαιωθείτε ότι έχετε τις κατάλληλες άδειες χρήσης για το SKU/συνδρομές. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [άδειες χρήσης SKU/συνδρομές](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Ελέγξτε τα δικαιώματα που απαιτούνται για να ενεργοποιήσετε τη διαχείριση συσκευών, να αποκτήσετε πρόσβαση στη σελίδα εγγραφής ή να ενεργοποιήσετε/απενεργοποιήσετε την παρακολούθηση συσκευών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Εγγράψτε συσκευές στη Διαχείριση συσκευών, ακολουθώντας τη διαδικασία εγγραφής συσκευών. Εάν δεν έχετε την επιλογή "Εγγραφή συσκευών" (προεπισκόπηση) στην περιοχή **Ρυθμίσεις** συμμόρφωσης M365, βεβαιωθείτε ότι έχετε την κατάλληλη άδεια χρήσης και τα δικαιώματα που αναφέρονται παραπάνω. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Δημιουργήστε πολιτικές DLP για την προστασία των ευαίσθητων στοιχείων σας. Για πληροφορίες, ανατρέξτε στο θέμα [Σενάρια πολιτικής DLP τελικών σημείων](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Για περισσότερες πληροφορίες σχετικά με τα DLP τελικών σημείων της Microsoft, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την αποτροπή απώλειας δεδομένων τελικών σημείων του Microsoft 365 (προεπισκόπηση)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Σημαντικά βήματα συλλογής δεδομένων, εάν απαιτείται υποστήριξη:**

1. Κατέβασμα της Προεπισκόπησης ανάλυσης προγράμματος-πελάτη MDATP από το [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Εκτελέστε το εργαλείο ως διαχειριστής από το παράθυρο cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Όταν σας ζητηθεί η ερώτηση "Εισαγάγετε τον αριθμό των λεπτών για τη συλλογή ανιχνεύσεων:", εισαγάγετε τον αριθμό των λεπτών που απαιτούνται για την εκτέλεση του σεναρίου
5. Εκτέλεση του σεναρίου

Συλλέξτε την έξοδο του αρχείου zip που θα δοθεί στον συνεργάτη υποστήριξης.
