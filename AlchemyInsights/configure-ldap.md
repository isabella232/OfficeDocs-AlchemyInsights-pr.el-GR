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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090412"
---
# <a name="configure-ldap"></a>Ρύθμιση παραμέτρων LDAP

Για να ρυθμίσετε τις παραμέτρους του LDAP, κάντε τα εξής:

1. Ελέγξτε την κατάσταση του τομέα σας στην [πύλη Azure.](https://aka.ms/aadds-health)
1. Βεβαιωθείτε ότι είναι διαθέσιμη μια έγκυρη συνδρομή azure AD και ότι οι υπηρεσίες τομέα Azure AD έχουν ενεργοποιηθεί.
1. Το πιστοποιητικό που απαιτείται για την ενεργοποίηση του ασφαλούς LDAP πρέπει να λαμβάνεται από μια αξιόπιστη δημόσια αρχή έκδοσης πιστοποιητικών ή να είναι ένα αυτο-υπογεγραμμένο πιστοποιητικό.
1. Βεβαιωθείτε ότι το πιστοποιητικό ακολουθεί τις απαιτούμενες [οδηγίες.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Μη έγκυρο πιστοποιητικό**
1. Για να ανανεώσετε ένα πιστοποιητικό, ακολουθήστε τα βήματα για να δημιουργήσετε ένα νέο πιστοποιητικό και να επαναφορτώσετε: [Ρύθμιση παραμέτρων LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Για να επιλύσετε ένα γνωστό πρόβλημα με τις ειδοποιήσεις Secure LDAP στις υπηρεσίες τομέα Azure Active directory, ανατρέξτε στο θέμα [Επίλυση ειδοποιήσεων LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
