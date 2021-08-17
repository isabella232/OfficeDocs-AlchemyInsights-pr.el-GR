---
title: Πολιτικές κωδικού πρόσβασης
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040830"
---
# <a name="password-policies"></a>Πολιτικές κωδικού πρόσβασης

**Έχω προβλήματα με την πολιτική κωδικού πρόσβασης για ένα χρήστη**

- Η πολιτική κωδικού πρόσβασης για ένα χρήστη εξαρτάται από το εάν ο χρήστης είναι μόνο στο cloud ή στην εσωτερική εγκατάσταση.
- Μόνο οι χρήστες στο cloud πρέπει να επιλέξουν έναν κωδικό πρόσβασης που πληροί τις απαιτήσεις αυτού του άρθρου: [Πολιτικές κωδικού πρόσβασης που ισχύουν μόνο για λογαριασμούς χρηστών cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Οι χρήστες εσωτερικής εγκατάστασης πρέπει να επιλέξουν έναν κωδικό πρόσβασης που πληροί τις απαιτήσεις εσωτερικής εγκατάστασης. Εάν ένας χρήστης εσωτερικής εγκατάστασης δεν μπορεί να ορίσει τον κωδικό πρόσβασής του, ελέγξτε τις απαιτήσεις εσωτερικής εγκατάστασης.

**Δεν ξέρω πώς μπορείτε να ορίσετε ή να ελέγξετε τις πολιτικές λήξης κωδικού πρόσβασης**

- Μπορείτε να ορίσετε και να ελέγξετε την πολιτική λήξης για χρήστες cloud στο μισθωτή σας χρησιμοποιώντας το PowerShell. Ακολουθήστε τις οδηγίες σε αυτό το άρθρο: [Ορίστε ή ελέγξτε τις πολιτικές κωδικού πρόσβασης χρησιμοποιώντας το PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Η πολιτική λήξης κωδικού πρόσβασης για τους χρήστες εσωτερικής εγκατάστασης έχει οριστεί στο AD εσωτερικής εγκατάστασης.

**Άλλες χρήσιμες συνδέσεις:**
- [Γρήγορα αποτελέσματα με την επαναφορά κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Αντιμετώπιση προβλημάτων επαναφοράς κωδικού πρόσβασης που ξεκίνησε από το διαχειριστή](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
