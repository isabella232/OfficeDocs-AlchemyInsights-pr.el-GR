---
title: Αντιμετώπιση προβλημάτων με το Microsoft Defender για το Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801407"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Αντιμετώπιση προβλημάτων με το Office 365 ATP

- **Καθυστερήσεις ειδοποίησης με την παράδοση μηνυμάτων ηλεκτρονικού ταχυδρομείου** ; Δοκιμάστε να χρησιμοποιήσετε την επιλογή δυναμικής παράδοσης για τις πολιτικές των ασφαλών συνημμένων ATP. Αυτό θα αποτρέψει καθυστερήσεις παράδοσης μηνυμάτων ηλεκτρονικού ταχυδρομείου ενώ προστατεύει τους παραλήπτες από κακόβουλα αρχεία.
- **Θέλετε να αναφέρετε ψευδώς θετικά ή ψευδή αρνητικά** ; Χρησιμοποιήστε αυτήν τη σύνδεση για να υποβάλετε το αρχείο σας για ανάλυση: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- Γνωρίζατε **ότι μπορείτε να ενεργοποιήσετε την προστασία των ασφαλών συνδέσεων ATP για μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ ατόμων στην εταιρεία σας** ; Ακολουθήστε τα εξής βήματα:
    1. Μεταβείτε στην https://protection.office.com και πραγματοποιήστε είσοδο.
    2. Μεταβείτε στις **Threat management**  >  **Policy**  >  **ασφαλείς συνδέσεις** της πολιτικής διαχείρισης απειλών.
    3. Στην περιοχή **πολιτικές που ισχύουν για συγκεκριμένους παραλήπτες** , επεξεργαστείτε (ή προσθέστε) μια πολιτική.
    4. Επιλέξτε **εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός του οργανισμού** .
    5. Αποθηκεύστε την πολιτική σας και επιτρέψτε περίπου 30 λεπτά για να λειτουργήσουν οι αλλαγές σας μέσω του Datacenter.
- Για να λάβετε περισσότερη βοήθεια με το ATP, ανατρέξτε στο θέμα [Microsoft Defender για το Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).