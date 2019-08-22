---
title: Ημερήσια ηλεκτρονικού ταχυδρομείου έγινε υπέρβαση του ορίου. Αναστολή ροής εργασίας.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514452"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Υπέρβαση του ορίου ημερήσιων ηλεκτρονικού ταχυδρομείου. Αναστολή ροής εργασίας.

Αυτό το σφάλμα ενδέχεται να εμφανιστούν στα ακόλουθα σενάρια:

- Μπορείτε να έχετε μια ροή εργασίας σε ηλεκτρονική SharePoint που χρησιμοποιεί το SharePoint 2010 ή τύπος πλατφόρμας ροής εργασίας του SharePoint 2013.
- Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερα από 200 χρήστες κάθε φορά, περισσότερες από 10.000 παραλήπτες ανά ημέρα είτε περισσότερα από 30 μηνύματα ανά λεπτό.
- Κατά την εκτέλεση της ροής εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρήσετε την ακόλουθη συμπεριφορά:
    - Χρήση του τύπου πλατφόρμα SharePoint 2013 μιας ροής εργασίας, μεταβείτε στη σελίδα " **Κατάσταση ροής εργασίας** ". Στη σελίδα "Κατάσταση ροής εργασίας", η **Εσωτερική κατάσταση** έχει οριστεί σε **αποτελέσματα**και το παράθυρο πληροφοριών εμφανίζει **δεν είναι δυνατή η αποστολή σε παραλήπτη**.

Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τις παραμέτρους ροής εργασίας για να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνουν το [Exchange Online όρια του αποστολέα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλετε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Office 365, μια ομάδα διανομής ή ομάδα ασφαλείας αλληλογραφίας ενεργοποιημένη ή στείλτε το μήνυμα σε λιγότερα από 200 παραλήπτες ταυτόχρονα.


Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Σχετικά θέματα
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Του SharePoint και ροής](https://flow.microsoft.com/blog/sharepoint-and-flow/) 