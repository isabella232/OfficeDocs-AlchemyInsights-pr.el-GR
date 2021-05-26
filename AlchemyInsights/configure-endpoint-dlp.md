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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657929"
---
# <a name="configure-endpoint-dlp"></a>Ρύθμιση παραμέτρων DLP τελικών σημείων

Τα DLP τελικών σημείων της Microsoft σάς επιτρέπουν να επεκτείνετε τη δυνατότητα προστασίας και παρακολούθησης DLP στις ευαίσθητες πληροφορίες σε συσκευές Windows 10. Αφού οι συσκευές εγγραφούν στη διαχείριση συσκευών, μπορείτε να δημιουργήσετε πολιτικές DLP για την επιβολή ασφαλιστικών ενεργειών σε στοιχεία. Η "Εξερεύνηση δραστηριότητας" μπορεί να χρησιμοποιηθεί για την παρακολούθηση της δραστηριότητας για ευαίσθητα στοιχεία. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών στη διαχείριση συσκευών](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Για να ξεκινήσετε με τα DLP τελικών σημείων:

- Βεβαιωθείτε ότι έχετε τις κατάλληλες άδειες χρήσης για το SKU/συνδρομές. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [άδειες χρήσης SKU/συνδρομές](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Ελέγξτε τα δικαιώματα που απαιτούνται για να ενεργοποιήσετε τη διαχείριση συσκευών, να αποκτήσετε πρόσβαση στη σελίδα εγγραφής ή να ενεργοποιήσετε/απενεργοποιήσετε την παρακολούθηση συσκευών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Εγγράψτε συσκευές στη Διαχείριση συσκευών, ακολουθώντας τη διαδικασία εγγραφής συσκευών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Δημιουργήστε πολιτικές DLP για την προστασία των ευαίσθητων στοιχείων σας. Για πληροφορίες, ανατρέξτε στο θέμα [Σενάρια πολιτικής DLP τελικών σημείων](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Για περισσότερες πληροφορίες σχετικά με τα DLP τελικών σημείων της Microsoft, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την αποτροπή απώλειας δεδομένων τελικών σημείων του Microsoft 365 (προεπισκόπηση)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Σημαντικά βήματα συλλογής δεδομένων, εάν απαιτείται υποστήριξη:**

1. Λήψη [MDATP Προγράμματος-πελάτη Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Εκτελέστε το εργαλείο ως διαχειριστής από το παράθυρο cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Όταν σας ζητηθεί με το enter ο αριθμός των λεπτών για τη συλλογή **ανιχνεύει:**, πληκτρολογήστε τον αριθμό των λεπτών που απαιτούνται για την εκτέλεση του σεναρίου.
1. Εκτελέστε το σενάριο.

Συλλέξτε το αποτέλεσμα του αρχείου Zip για να το δώσετε στον εκπρόσωπο υποστήριξης.
