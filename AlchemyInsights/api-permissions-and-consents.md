---
title: Δικαιώματα API και συγκατάθεση
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932097"
---
# <a name="api-permissions-and-consent"></a>Δικαιώματα API και συγκατάθεση

Οι εφαρμογές που ενοποιούνται με Πλατφόρμα ταυτοτήτων της Microsoft ακολουθούν ένα μοντέλο εξουσιοδότησης που παρέχει στους χρήστες και τους διαχειριστές τον έλεγχο του πώς μπορούν να έχουν πρόσβαση στα δεδομένα. Η υλοποίηση του μοντέλου εξουσιοδότησης έχει ενημερωθεί στο Πλατφόρμα ταυτοτήτων της Microsoft τελικό σημείο. Αλλάζει τον τρόπο με τον οποίο μια εφαρμογή πρέπει να αλληλεπιδρά με Πλατφόρμα ταυτοτήτων της Microsoft. [Τα δικαιώματα και η συγκατάθεση στο Πλατφόρμα ταυτοτήτων της Microsoft τελικό](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) σημείο καλύπτει τις βασικές έννοιες αυτού του μοντέλου εξουσιοδότησης, συμπεριλαμβανομένων των εμβέλειων, των δικαιωμάτων και της συγκατάθεσης.

Το [Azure Active Directory (Azure AD) διευκολύνει](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) την ανάπτυξη εφαρμογών web πολλών μισθωτών και εγγενών εφαρμογών-πελατών. Αυτές οι εφαρμογές επιτρέπουν την είσοδο από λογαριασμούς χρηστών από ένα μισθωτή Azure AD που είναι διαφορετικός από αυτόν όπου έχει καταχωρηθεί η εφαρμογή. Μπορεί επίσης να χρειαστεί να αποκτήσουν πρόσβαση σε API web, όπως το API του Microsoft Graph (για να αποκτήσουν πρόσβαση στο Azure AD, το Intune και τις υπηρεσίες στο Microsoft 365) και άλλα API του Υπηρεσίες της Microsoft, εκτός από τα δικά σας API web.

