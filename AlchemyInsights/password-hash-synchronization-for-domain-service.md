---
title: Συγχρονισμός hash κωδικού πρόσβασης για την υπηρεσία τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177491"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Συγχρονισμός hash κωδικού πρόσβασης για την υπηρεσία τομέα

**Εάν η παρουσία azure AD DS σάς ζητά να ενεργοποιήσετε το συγχρονισμό hash κωδικού πρόσβασης**

Αντιμετωπίζετε ένα σενάριο στο οποίο εκτελείτε ένα υβριδικό περιβάλλον με χρήστες που συγχρονίζονται από ένα περιβάλλον υπηρεσιών τομέα Azure Active Directory (AD DS) εσωτερικής εγκατάστασης. Αυτό το σενάριο αντιμετωπίζεται παρά το γεγονός ότι έχετε συγχρονισμό hash κωδικού πρόσβασης από τις υπηρεσίες AD DS εσωτερικής εγκατάστασης στο μισθωτή azure AD.

**Αιτία**

Αυτό συμβαίνει επειδή το Azure AD Connect από προεπιλογή δεν συγχρονίζει hashes κωδικού πρόσβασης LAN Manager νέας τεχνολογίας παλαιού τύπου (NTLM) και Kerberos που είναι απαραίτητοι για το Azure AD DS.

**Λύση** 

Θα πρέπει να ρυθμίσετε τις παραμέτρους του Azure AD Connect για να συγχρονίσετε αυτούς τους hashes κωδικού πρόσβασης που απαιτούνται για τον έλεγχο ταυτότητας NTLM και Kerberos.

Αφού ρυθμιστούν οι παράμετροι του Azure AD Connect, ένα συμβάν δημιουργίας ή αλλαγής κωδικού πρόσβασης εσωτερικής εγκατάστασης συγχρονίζει επίσης τον κωδικό πρόσβασης παλαιού τύπου στο Azure AD. Ανατρέξτε [εδώ για](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) περισσότερες πληροφορίες σχετικά με αυτό το θέμα και για οδηγίες σχετικά με τον τρόπο ενεργοποίησης του συγχρονισμού κωδικών πρόσβασης σε υβριδικά περιβάλλοντα Azure AD DS.