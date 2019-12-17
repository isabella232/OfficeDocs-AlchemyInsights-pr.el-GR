---
title: Έγινε υπέρβαση του ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας έχει ανασταλεί.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053117"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Έγινε υπέρβαση του ορίου ημερήσιων μηνυμάτων ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας έχει ανασταλεί.

Αυτό το σφάλμα μπορεί να παραληφθεί στα ακόλουθα σενάρια:

- Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί το SharePoint 2010 ή τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2013.
- Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα, ή περισσότερα από 30 μηνύματα ανά λεπτό.
- Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε την ακόλουθη συμπεριφορά:
    - Για μια ροή εργασίας χρησιμοποιώντας τον τύπο πλατφόρμας του SharePoint 2013, μεταβείτε στη σελίδα **κατάσταση ροής εργασίας** . Στη σελίδα "κατάσταση ροής εργασίας", η **εσωτερική κατάσταση** έχει οριστεί σε **Έναρξη**και το πλαίσιο πληροφοριών εμφανίζει **δεν είναι δυνατή η αποστολή σε έναν παραλήπτη**.

Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τη ροή εργασίας σας για να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνει τα [όρια αποστολέα του Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλτε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Office 365, μια ομάδα διανομής ή μια υπηρεσία ασφαλείας με δυνατότητα αλληλογραφίας ή στείλτε το μήνυμά σας σε λιγότερους από 200 παραλήπτες κάθε φορά.


Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Σχετικά θέματα
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και ροή](https://flow.microsoft.com/blog/sharepoint-and-flow/) 