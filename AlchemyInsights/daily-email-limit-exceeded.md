---
title: Υπέρβαση ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας αναστέλλεται.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914651"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Υπέρβαση ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας αναστέλλεται.

Αυτό το σφάλμα μπορεί να εμφανιστεί στα ακόλουθα σενάρια:

- Έχετε μια ροή εργασιών στο SharePoint Online που χρησιμοποιεί τον τύπο πλατφόρμας ροής εργασίας SharePoint 2010 ή SharePoint 2013.
- Η ροή εργασίας έχει ρυθμιστεί ώστε να στέλνει ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα ή περισσότερα από 30 μηνύματα ανά λεπτό.
- Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρήσετε την ακόλουθη συμπεριφορά:
    - Για μια ροή εργασίας που SharePoint τύπο πλατφόρμας 2013, μεταβείτε στη σελίδα "Κατάσταση **ροής εργασίας".** Στη σελίδα "Κατάσταση  ροής εργασίας", η "Εσωτερική κατάσταση" έχει οριστεί σε "Ξεκίνησε" και το πλαίσιο πληροφοριών εμφανίζει την ένδειξη **"Δεν είναι δυνατή η αποστολή σε παραλήπτη".**

Για να επιλύσετε αυτό το πρόβλημα, ρυθμίστε τις παραμέτρους της ροής εργασίας σας για την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου [χωρίς να υπερβαίνει Exchange Online όρια αποστολέα.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλτε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Microsoft 365, μια ομάδα διανομής ή μια ομάδα ασφαλείας με δυνατότητα αλληλογραφίας ή στείλτε το μήνυμα σε λιγότερους από 200 παραλήπτες κάθε φορά.


Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Σχετικά θέματα
- [Δημιουργία Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 