---
title: Αντιμετώπιση προβλημάτων πιστοποιητικού υπογραφής SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693421"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Αντιμετώπιση προβλημάτων πιστοποιητικού υπογραφής SAML

Για να επιλύσετε το ζήτημα του πιστοποιητικού υπογραφής SAML, εκτελέστε τα ακόλουθα προτεινόμενα βήματα:

1. Όταν προσθέτετε μια εταιρική εφαρμογή που υποστηρίζει SSO, το Azure θα δημιουργήσει ένα πιστοποιητικό που ονομάζεται [πιστοποιητικό υπογραφής SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Αυτό το πιστοποιητικό έχει ημερομηνία λήξης 3 ετών. Για να αλλάξετε την ημερομηνία λήξης του πιστοποιητικού, ανατρέξτε στο θέμα "Προσαρμογή της ημερομηνίας λήξης για το πιστοποιητικό ομοσπονδίας και [αναδίφτε το σε νέο πιστοποιητικό".](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Το Azure θα χρησιμοποιήσει αυτό το πιστοποιητικό για να υπογράψει τα διακριτικά SAML που ζητούνται από την εφαρμογή και να τα στείλει στην εφαρμογή για μια επιτυχημένη SSO. Για να ολοκληρωθεί αυτό, κάντε λήψη του πιστοποιητικού από την πύλη Azure και στείλτε το στον προμηθευτή της εφαρμογής για να ολοκληρώσετε τη διαδικασία SSO.

Αφού ολοκληρωθεί αυτή η διαδικασία, η εφαρμογή σας θα εμπιστευτεί αυτό το πιστοποιητικό και όλα τα διακριτικά SAML που είναι υπογεγραμμένα από αυτό το πιστοποιητικό θα γίνουν αποδεκτά από την εφαρμογή.

3. Εάν λήξει αυτό το πιστοποιητικό, δημιουργήστε ένα νέο πιστοποιητικό, ενημερώστε το στον προμηθευτή της εφαρμογής και, στη συνέχεια, ενεργές στην πλευρά Azure. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Ανανέωση πιστοποιητικού που σύντομα θα λήξει".](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Εάν λήξει το πιστοποιητικό, ο χρήστης δεν θα αποκλειστεί.

4. [Προσθέστε μια διεύθυνση ηλεκτρονικού ταχυδρομείου για να λαμβάνετε](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) ειδοποιήσεις πριν από τη λήξη του τρέχοντος πιστοποιητικού.

> [!NOTE]
> Το βήμα 4 είναι προαιρετικό.

5. Αλλάξτε τις επιλογές υπογραφής πιστοποιητικών SAML μιας εφαρμογής και τον αλγόριθμο υπογραφής πιστοποιητικού. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Αλλαγή επιλογών υπογραφής πιστοποιητικού και αλγόριθμος υπογραφής".](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

