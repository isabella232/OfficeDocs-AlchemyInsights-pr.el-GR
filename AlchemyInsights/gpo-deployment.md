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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427254"
---
# <a name="gpo-deployment"></a>Ανάπτυξη GPO

Η διαχείριση των ρυθμίσεων για αντικείμενα χρηστών και υπολογιστών στις υπηρεσίες τομέα Azure Active Directory (Azure AD DS) γίνεται συχνά με τη χρήση αντικειμένων πολιτικής ομάδας (GPOs). Το Azure AD DS περιλαμβάνει ενσωματωμένα GPOs για τους χρήστες AADDC και τα κοντέινερ υπολογιστών AADDC. Μπορείτε να προσαρμόσετε αυτά τα ενσωματωμένα GPOs για να ρυθμίσετε τις παραμέτρους της πολιτικής ομάδας ανάλογα με τις ανάγκες για το περιβάλλον σας. Τα μέλη της ομάδας διαχειριστών DC του Azure AD έχουν δικαιώματα διαχείρισης πολιτικής ομάδας στον τομέα Azure AD DS και μπορούν επίσης να δημιουργήσουν προσαρμοσμένα GPOs και εταιρικές μονάδες (OUs). Για περισσότερες πληροφορίες σχετικά με την πολιτική ομάδας και τον τρόπο που λειτουργεί, ανατρέξτε στο θέμα ["Επισκόπηση πολιτικής ομάδας".](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Σε ένα υβριδικό περιβάλλον, οι πολιτικές ομάδας που έχουν ρυθμιστεί σε περιβάλλον AD DS εσωτερικής εγκατάστασης δεν συγχρονίζονται με το Azure AD DS. Για να ορίσετε ρυθμίσεις παραμέτρων για χρήστες ή υπολογιστές στο Azure AD DS, επεξεργαστείτε ένα από τα προεπιλεγμένα GPOs ή δημιουργήστε ένα προσαρμοσμένο GPO.

Αυτό το [άρθρο "Διαχείριση](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) πολιτικής ομάδας" σάς δείχνει πώς μπορείτε να εγκαταστήσετε τα εργαλεία διαχείρισης πολιτικής ομάδας, πώς μπορείτε να επεξεργαστείτε τα ενσωματωμένα GPOs και πώς μπορείτε να δημιουργήσετε προσαρμοσμένα GPOs.
