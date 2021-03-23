---
title: Αντιμετώπιση προβλημάτων κωδικών σφάλματος ελέγχου ταυτότητας και εξουσιοδότησης azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036505"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Αντιμετώπιση προβλημάτων κωδικών σφάλματος ελέγχου ταυτότητας και εξουσιοδότησης azure AD (AADSTS)

Για να επιλύσετε τους κωδικούς σφαλμάτων ελέγχου ταυτότητας και εξουσιοδότησης AAD (AADSTS), εκτελέστε τα ακόλουθα προτεινόμενα βήματα:

1. **Χειρισμός κωδικών σφάλματος στην εφαρμογή σας**

- Η **προδιαγραφή OAuth2.0** παρέχει οδηγίες σχετικά με τον τρόπο χειρισμού σφαλμάτων κατά τον έλεγχο ταυτότητας, χρησιμοποιώντας https://tools.ietf.org/html/rfc6749#section-5.2 το τμήμα σφάλματος της απόκρισης σφάλματος.

    - **σφάλμα**: Μια συμβολοσειρά κωδικού σφάλματος που μπορεί να χρησιμοποιηθεί για την ταξινόμηση τύπων σφαλμάτων που προκύπτουν και θα πρέπει να χρησιμοποιηθεί για την αντίδραση σε σφάλματα.
    - Το **πεδίο** σφάλματος έχει πολλές πιθανές τιμές - εξετάστε τις συνδέσεις τεκμηρίωσης πρωτοκόλλου και τις προδιαγραφές OAuth 2.0 για περισσότερες πληροφορίες σχετικά με συγκεκριμένα σφάλματα και τον τρόπο αντίδρασης σε αυτά.

- Ακολουθεί ένα δείγμα απόκρισης σφάλματος:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Πληροφορίες κώδικα τρέχοντος σφάλματος αναζήτησης**

- Οι κωδικοί σφάλματος και τα μηνύματα υπόκεινται σε αλλαγή. Για τις πιο τρέχουσες πληροφορίες, ανατρέξτε στη σελίδα για να βρείτε περιγραφές σφαλμάτων https://login.microsoftonline.com/error AADSTS, επιδιορθώσεις και ορισμένες προτεινόμενες λύσεις.
- Μπορείτε επίσης να αναζητήσετε και να αντιμετωπίσετε τους [κωδικούς σφάλματος AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) που παρατίθενται στο άρθρο "Έλεγχος ταυτότητας [azure AD" και κωδικοί σφάλματος εξουσιοδότησης.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Λήψη βοήθειας**

- [Επιλογές υποστήριξης και](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) βοήθειας για προγραμματιστές - Εάν χρειάζεστε μια απάντηση σε μια ερώτηση ή βοήθεια για την επίλυση ενός προβλήματος που δεν καλύπτεται στην τεκμηρίωσή μας, ίσως είναι ώρα να επικοινωνήστε με ειδικούς για βοήθεια. Αυτό το άρθρο παρέχει διάφορες προτάσεις για τη λήψη απαντήσεων στις ερωτήσεις σας καθώς αναπτύσσετε εφαρμογές που ενοποιούνται με την πλατφόρμα ταυτότητας της Microsoft.








