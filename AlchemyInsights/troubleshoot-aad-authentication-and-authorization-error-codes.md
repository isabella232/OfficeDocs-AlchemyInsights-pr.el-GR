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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="2ac8e-102">Αντιμετώπιση προβλημάτων κωδικών σφάλματος ελέγχου ταυτότητας και εξουσιοδότησης azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="2ac8e-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="2ac8e-103">Για να επιλύσετε τους κωδικούς σφαλμάτων ελέγχου ταυτότητας και εξουσιοδότησης AAD (AADSTS), εκτελέστε τα ακόλουθα προτεινόμενα βήματα:</span><span class="sxs-lookup"><span data-stu-id="2ac8e-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="2ac8e-104">**Χειρισμός κωδικών σφάλματος στην εφαρμογή σας**</span><span class="sxs-lookup"><span data-stu-id="2ac8e-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="2ac8e-105">Η **προδιαγραφή OAuth2.0** παρέχει οδηγίες σχετικά με τον τρόπο χειρισμού σφαλμάτων κατά τον έλεγχο ταυτότητας, χρησιμοποιώντας https://tools.ietf.org/html/rfc6749#section-5.2 το τμήμα σφάλματος της απόκρισης σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="2ac8e-106">**σφάλμα**: Μια συμβολοσειρά κωδικού σφάλματος που μπορεί να χρησιμοποιηθεί για την ταξινόμηση τύπων σφαλμάτων που προκύπτουν και θα πρέπει να χρησιμοποιηθεί για την αντίδραση σε σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="2ac8e-107">Το **πεδίο** σφάλματος έχει πολλές πιθανές τιμές - εξετάστε τις συνδέσεις τεκμηρίωσης πρωτοκόλλου και τις προδιαγραφές OAuth 2.0 για περισσότερες πληροφορίες σχετικά με συγκεκριμένα σφάλματα και τον τρόπο αντίδρασης σε αυτά.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="2ac8e-108">Ακολουθεί ένα δείγμα απόκρισης σφάλματος:</span><span class="sxs-lookup"><span data-stu-id="2ac8e-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="2ac8e-109">**Πληροφορίες κώδικα τρέχοντος σφάλματος αναζήτησης**</span><span class="sxs-lookup"><span data-stu-id="2ac8e-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="2ac8e-110">Οι κωδικοί σφάλματος και τα μηνύματα υπόκεινται σε αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="2ac8e-111">Για τις πιο τρέχουσες πληροφορίες, ανατρέξτε στη σελίδα για να βρείτε περιγραφές σφαλμάτων https://login.microsoftonline.com/error AADSTS, επιδιορθώσεις και ορισμένες προτεινόμενες λύσεις.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="2ac8e-112">Μπορείτε επίσης να αναζητήσετε και να αντιμετωπίσετε τους [κωδικούς σφάλματος AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) που παρατίθενται στο άρθρο "Έλεγχος ταυτότητας [azure AD" και κωδικοί σφάλματος εξουσιοδότησης.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="2ac8e-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="2ac8e-113">**Λήψη βοήθειας**</span><span class="sxs-lookup"><span data-stu-id="2ac8e-113">**Get Help**</span></span>

- <span data-ttu-id="2ac8e-114">[Επιλογές υποστήριξης και](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) βοήθειας για προγραμματιστές - Εάν χρειάζεστε μια απάντηση σε μια ερώτηση ή βοήθεια για την επίλυση ενός προβλήματος που δεν καλύπτεται στην τεκμηρίωσή μας, ίσως είναι ώρα να επικοινωνήστε με ειδικούς για βοήθεια.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="2ac8e-115">Αυτό το άρθρο παρέχει διάφορες προτάσεις για τη λήψη απαντήσεων στις ερωτήσεις σας καθώς αναπτύσσετε εφαρμογές που ενοποιούνται με την πλατφόρμα ταυτότητας της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ac8e-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








