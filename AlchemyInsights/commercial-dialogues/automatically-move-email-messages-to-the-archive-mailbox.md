---
title: Αυτόματη μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059226"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Αυτόματη μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

Δείτε πώς μπορείτε να ρυθμίσετε μια πολιτική για την αυτόματη μετακίνηση του παλιού ηλεκτρονικού ταχυδρομείου ενός χρήστη στο γραμματοκιβώτιο αρχειοθέτησης:

1. Μεταβείτε [**στην "& Αρχειοθέτηση διαχείρισης**](https://go.microsoft.com/fwlink/p/?linkid=2077143)δεδομένων  >  **συμμόρφωσης"** για να  >   επαληθεύσετε ότι έχει ενεργοποιηθεί ένα γραμματοκιβώτιο αρχειοθέτησης για το χρήστη. Εάν δεν το έχει κάνει, κάντε κλικ στην επιλογή **"Ενεργοποίηση"** **και, στη συνέχεια, "Ναι"** στο πλαίσιο προειδοποίησης.
2. Μεταβείτε [**στο Exchange διαχείρισης > διαχείρισης συμμόρφωσης > ετικέτες διατήρησης.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Επιλέξτε το εικονίδιο + και, στη **συνέχεια, επιλέξτε αυτόματη εφαρμογή σε ολόκληρο το γραμματοκιβώτιο.**
4. Αντιστοιχίστε ένα όνομα στην ετικέτα διατήρησης και επιλέξτε **"Μετακίνηση στην Αρχειοθήκη".** Για την περίοδο διατήρησης, εισαγάγετε το χρόνο που θέλετε, όπως 90 ημέρες. Επιλέξτε **Αποθήκευση**.
5. Τώρα δημιουργήστε μια πολιτική διατήρησης: επιλέξτε **πολιτικές διατήρησης,** επιλέξτε το εικονίδιο για να προσθέσετε μια νέα πολιτική.
6. Αντιστοιχίστε ένα όνομα στην πολιτική διατήρησης και, στη συνέχεια, κάντε κλικ και κάντε κύλιση για να βρείτε και να προσθέσετε την ετικέτα διατήρησης που μόλις δημιουργήσατε. Επιλέξτε **Αποθήκευση**.
7. Τέλος, εφαρμόστε την πολιτική διατήρησης στο γραμματοκιβώτιο του χρήστη: εξακολουθείτε να Exchange, μεταβείτε **στα γραμματοκιβώτια**  >  **παραληπτών.** Επιλέξτε όλους τους χρήστες στους οποίοι θέλετε να εφαρμόσετε την πολιτική και, στη συνέχεια, επιλέξτε **"Επεξεργασία"** (το εικονίδιο μολυβιού).
8. Στο παράθυρο διαλόγου, κάντε κλικ στις δυνατότητες **γραμματοκιβωτίου.** Στην **περιοχή "Πολιτική** διατήρησης", εφαρμόστε την πολιτική που μόλις δημιουργήσατε > **Αποθήκευση.**
9. Για οδηγίες σχετικά με την εφαρμογή της πολιτικής σε όλους τους χρήστες, ανατρέξτε στο θέμα [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
