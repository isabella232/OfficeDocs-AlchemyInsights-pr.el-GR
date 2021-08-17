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
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892799"
---
# <a name="configure-endpoint-dlp"></a>Ρύθμιση παραμέτρων DLP τελικών σημείων

Τα DLP τελικών σημείων της Microsoft σάς επιτρέπουν να επεκτείνετε τη δυνατότητα προστασίας και παρακολούθησης DLP στις ευαίσθητες πληροφορίες σε συσκευές Windows 10. Αφού οι συσκευές εγγραφούν στη διαχείριση συσκευών, μπορείτε να δημιουργήσετε πολιτικές DLP για την επιβολή ασφαλιστικών ενεργειών σε στοιχεία. Η "Εξερεύνηση δραστηριότητας" μπορεί να χρησιμοποιηθεί για την παρακολούθηση της δραστηριότητας για ευαίσθητα στοιχεία. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών στη διαχείριση συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Για να ξεκινήσετε με τα DLP τελικών σημείων:

- Βεβαιωθείτε ότι έχετε τις κατάλληλες άδειες χρήσης για το SKU/συνδρομές. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [άδειες χρήσης SKU/συνδρομές](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Ελέγξτε τα δικαιώματα που απαιτούνται για να ενεργοποιήσετε τη διαχείριση συσκευών, να αποκτήσετε πρόσβαση στη σελίδα εγγραφής ή να ενεργοποιήσετε/απενεργοποιήσετε την παρακολούθηση συσκευών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Εγγράψτε συσκευές στη Διαχείριση συσκευών, ακολουθώντας τη διαδικασία εγγραφής συσκευών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εγγραφή συσκευών](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Δημιουργήστε πολιτικές DLP για την προστασία των ευαίσθητων στοιχείων σας. Για πληροφορίες, ανατρέξτε στο θέμα [Σενάρια πολιτικής DLP τελικών σημείων](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Για περισσότερες πληροφορίες σχετικά με τα DLP τελικών σημείων της Microsoft, ανατρέξτε στο θέμα [Μάθετε περισσότερα σχετικά με την αποτροπή απώλειας δεδομένων τελικών σημείων του Microsoft 365 (προεπισκόπηση)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Σημαντικά βήματα συλλογής δεδομένων, εάν απαιτείται υποστήριξη:**

1. Κάντε λήψη [του MDATP Client Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Εκτελέστε το εργαλείο ως διαχειριστής από το παράθυρο cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Όταν σας ζητηθεί με το enter ο αριθμός των λεπτών για τη συλλογή **ανιχνεύει:**, πληκτρολογήστε τον αριθμό των λεπτών που απαιτούνται για την εκτέλεση του σεναρίου.
1. Εκτελέστε το σενάριο.

Συλλέξτε το αποτέλεσμα του αρχείου Zip για να το δώσετε στον εκπρόσωπο υποστήριξης.
