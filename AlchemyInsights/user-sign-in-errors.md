---
title: Σφάλματα εισόδου χρήστη
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900992"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="6dd1c-102">Σφάλματα εισόδου χρήστη</span><span class="sxs-lookup"><span data-stu-id="6dd1c-102">User sign-in errors</span></span>

<span data-ttu-id="6dd1c-103">**Επίλυση προβλημάτων με το διαγνωστικό εισόδου**</span><span class="sxs-lookup"><span data-stu-id="6dd1c-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="6dd1c-104">Για να εντοπίσετε την αιτία ή τη διάγνωση προβλημάτων που σχετίζονται με την είσοδο του χρήστη, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="6dd1c-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="6dd1c-105">Εκκινήστε το [διαγνωστικό εισόδου](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="6dd1c-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="6dd1c-106">Εντοπίστε το συμβάν για ανάλυση, πληκτρολογώντας τις λεπτομέρειες που έχετε σχετικά με το χρήστη, την εφαρμογή, την ώρα εισόδου, το αναγνωριστικό αίτησης ή το αναγνωριστικό συσχέτισης.</span><span class="sxs-lookup"><span data-stu-id="6dd1c-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="6dd1c-107">Εξετάστε τα διαγνωστικά αποτελέσματα που δείχνουν τις λεπτομέρειες σχετικά με το τι συνέβη και ποιες ενέργειες μπορείτε να ακολουθήσετε για να κάνετε αλλαγές, εάν χρειάζονται αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="6dd1c-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="6dd1c-108">**Αναζητάτε πληροφορίες σχετικά με τους κωδικούς σφάλματος AADSTS που επιστρέφονται από την υπηρεσία διακριτικού ασφαλείας (STS) του Azure Active Directory (Azure AD);**</span><span class="sxs-lookup"><span data-stu-id="6dd1c-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="6dd1c-109">Διαβάστε [αυτό το άρθρο](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) για να εντοπίσετε περιγραφές σφαλμάτων του AADSTS, επιδιορθώσεις και ορισμένες προτεινόμενες λύσεις</span><span class="sxs-lookup"><span data-stu-id="6dd1c-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>