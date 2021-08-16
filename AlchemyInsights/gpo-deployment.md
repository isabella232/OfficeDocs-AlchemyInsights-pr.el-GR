---
title: Ανάπτυξη GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067840"
---
# <a name="gpo-deployment"></a>Ανάπτυξη GPO

Ρυθμίσεις για αντικείμενα χρηστών και υπολογιστών στις Azure Active Directory υπηρεσιών τομέα (Azure AD DS) συχνά χρησιμοποιούνται αντικείμενα πολιτικής ομάδας (GPO). Το Azure AD DS περιλαμβάνει ενσωματωμένα GGPOs για τους χρήστες AADDC και τα κοντέινερ υπολογιστών AADDC. Μπορείτε να προσαρμόσετε αυτά τα ενσωματωμένα GPO για να ρυθμίσετε τις παραμέτρους της πολιτικής ομάδας, ανάλογα με τις ανάγκες για το περιβάλλον σας. Τα μέλη της ομάδας διαχειριστών του Azure AD DC έχουν δικαιώματα διαχείρισης πολιτικής ομάδας στον τομέα Azure AD DS και μπορούν επίσης να δημιουργήσουν προσαρμοσμένα GPO και εταιρικές μονάδες (OUs). Για περισσότερες πληροφορίες σχετικά με την πολιτική ομάδας και τον τρόπο με τον οποίο λειτουργεί, ανατρέξτε στο [θέμα "Επισκόπηση πολιτικής ομάδας".](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Σε ένα υβριδικό περιβάλλον, οι πολιτικές ομάδας που έχουν ρυθμιστεί σε περιβάλλον AD DS εσωτερικής εγκατάστασης δεν συγχρονίζονται με το Azure AD DS. Για να ορίσετε ρυθμίσεις παραμέτρων για χρήστες ή υπολογιστές στο Azure AD DS, επεξεργαστείτε ένα από τα προεπιλεγμένα GPO ή δημιουργήστε ένα προσαρμοσμένο GPO.

Αυτό το [άρθρο "Διαχείριση](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) πολιτικής ομάδας" σάς δείχνει πώς μπορείτε να εγκαταστήσετε τα εργαλεία διαχείρισης πολιτικής ομάδας, πώς να επεξεργαστείτε τα ενσωματωμένα GGPOs και πώς μπορείτε να δημιουργήσετε προσαρμοσμένα GGPOs.
