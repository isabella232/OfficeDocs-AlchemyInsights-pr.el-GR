---
title: Δικαιώματα και συγκατάθεση API
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974603"
---
# <a name="api-permissions-and-consent"></a>Δικαιώματα και συγκατάθεση API

Οι εφαρμογές που ενσωματώνονται με την πλατφόρμα ταυτοτήτων της Microsoft ακολουθούν ένα μοντέλο εξουσιοδότησης που παρέχει στους χρήστες και τους διαχειριστές τον έλεγχο του τρόπου με τον οποίο είναι δυνατή η πρόσβαση στα δεδομένα. Η εφαρμογή του μοντέλου εξουσιοδότησης έχει ενημερωθεί στο τελικό σημείο της πλατφόρμας ταυτοτήτων της Microsoft. Αλλάζει τον τρόπο με τον οποίο μια εφαρμογή πρέπει να αλληλεπιδρά με την πλατφόρμα ταυτοτήτων της Microsoft. Τα [δικαιώματα και η συναίνεση στο τελικό σημείο της πλατφόρμας ταυτότητας της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) καλύπτουν τις βασικές έννοιες αυτού του μοντέλου εξουσιοδότησης, συμπεριλαμβανομένων των πεδίων, των δικαιωμάτων και της συγκατάθεσης.

Το [πλαίσιο συναίνεσης του Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) διευκολύνει την ανάπτυξη των εφαρμογών Web πολλών μισθωτών και των εγγενές πρόγραμμα-πελάτη. Αυτές οι εφαρμογές επιτρέπουν την είσοδο από τους λογαριασμούς χρηστών από έναν μισθωτή AD Azure που είναι διαφορετικός από αυτόν όπου έχει καταχωρηθεί η εφαρμογή. Ενδέχεται επίσης να χρειαστεί να αποκτήσουν πρόσβαση σε API Web, όπως το Microsoft Graph API (για να αποκτήσετε πρόσβαση στο Azure AD, το Intune και τις υπηρεσίες στο Microsoft 365) και στα API άλλων υπηρεσιών της Microsoft, εκτός από τα δικά σας API Web.

