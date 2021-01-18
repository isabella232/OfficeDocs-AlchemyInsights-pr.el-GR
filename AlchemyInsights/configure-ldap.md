---
title: Ρύθμιση παραμέτρων LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885160"
---
# <a name="configure-ldap"></a>Ρύθμιση παραμέτρων LDAP

Για να ρυθμίσετε τις παραμέτρους του LDAP, κάντε τα εξής:

1. Επιλέξτε την εύρυθμη λειτουργία του τομέα σας στην [πύλη Azure](https://aka.ms/aadds-health).
1. Βεβαιωθείτε ότι είναι διαθέσιμη μια έγκυρη συνδρομή Azure AD και ότι οι υπηρεσίες τομέα AD Azure έχουν ενεργοποιηθεί.
1. Το πιστοποιητικό που απαιτείται για την ενεργοποίηση του ασφαλούς LDAP πρέπει να λαμβάνεται από μια αξιόπιστη δημόσια αρχή έκδοσης πιστοποιητικών ή να είναι ένα πιστοποιητικό αυτόματης υπογραφής.
1. Βεβαιωθείτε ότι το πιστοποιητικό ακολουθεί τις απαιτούμενες [οδηγίες](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Μη έγκυρο πιστοποιητικό**
1. Για να ανανεώσετε ένα πιστοποιητικό, ακολουθήστε τα βήματα για να δημιουργήσετε ένα νέο πιστοποιητικό και να κάνετε ξανά αποστολή: [Ρύθμιση παραμέτρων LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Για να επιλύσετε ένα γνωστό πρόβλημα με ασφαλείς ειδοποιήσεις LDAP στις υπηρεσίες τομέα Active Directory Azure, ανατρέξτε στο θέμα [επίλυση ΕΙΔΟΠΟΙΉΣΕΩΝ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
