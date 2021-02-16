---
title: Πολιτική ομάδας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256716"
---
# <a name="group-policy"></a>Πολιτική ομάδας

Η διαχείριση των ρυθμίσεων για αντικείμενα χρηστών και υπολογιστών στις υπηρεσίες τομέα Azure Active Directory (Azure AD DS) γίνεται συχνά με τη χρήση αντικειμένων πολιτικής ομάδας (GPOs). Το Azure AD DS περιλαμβάνει ενσωματωμένα GPOs για τους χρήστες AADDC και τα κοντέινερ υπολογιστών AADDC. Μπορείτε να προσαρμόσετε αυτά τα ενσωματωμένα GPOs για να ρυθμίσετε τις παραμέτρους της πολιτικής ομάδας ανάλογα με τις ανάγκες για το περιβάλλον σας. Τα μέλη της ομάδας διαχειριστών DC του Azure AD έχουν δικαιώματα διαχείρισης πολιτικής ομάδας στον τομέα Azure AD DS και μπορούν επίσης να δημιουργήσουν προσαρμοσμένα GPOs και εταιρικές μονάδες (OUs). Για περισσότερες πληροφορίες σχετικά με την πολιτική ομάδας και τον τρόπο που λειτουργεί, ανατρέξτε στο θέμα ["Επισκόπηση πολιτικής ομάδας".](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Σε ένα υβριδικό περιβάλλον, οι πολιτικές ομάδας που έχουν ρυθμιστεί σε περιβάλλον AD DS εσωτερικής εγκατάστασης δεν συγχρονίζονται με το Azure AD DS. Για να ορίσετε ρυθμίσεις παραμέτρων για χρήστες ή υπολογιστές στο Azure AD DS, επεξεργαστείτε ένα από τα προεπιλεγμένα GPOs ή δημιουργήστε ένα προσαρμοσμένο GPO.

Αυτό το [άρθρο "Διαχείριση](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) πολιτικής ομάδας" σάς δείχνει πώς μπορείτε να εγκαταστήσετε τα εργαλεία διαχείρισης πολιτικής ομάδας, πώς μπορείτε να επεξεργαστείτε τα ενσωματωμένα GPOs και πώς μπορείτε να δημιουργήσετε προσαρμοσμένα GPOs.



