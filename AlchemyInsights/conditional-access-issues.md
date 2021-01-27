---
title: Προβλήματα πρόσβασης υπό όρους
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014790"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="6c6c2-102">Προβλήματα πρόσβασης υπό όρους</span><span class="sxs-lookup"><span data-stu-id="6c6c2-102">Conditional access issues</span></span>

<span data-ttu-id="6c6c2-103">**Επίλυση προβλημάτων με το διαγνωστικό εισόδου**</span><span class="sxs-lookup"><span data-stu-id="6c6c2-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="6c6c2-104">Μπορείτε να μάθετε γρήγορα τι συνέβη ή να διαγνώσετε προβλήματα που σχετίζονται με την είσοδο του χρήστη, χρησιμοποιώντας το [διαγνωστικό εισόδου](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="6c6c2-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="6c6c2-105">Εκκινήστε το διαγνωστικό εισόδου.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="6c6c2-106">Εντοπίστε το συμβάν για ανάλυση, πληκτρολογώντας τις λεπτομέρειες που έχετε σχετικά με το χρήστη, την εφαρμογή, την ώρα εισόδου, το αναγνωριστικό αίτησης ή το αναγνωριστικό συσχέτισης.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="6c6c2-107">Εξετάστε τα διαγνωστικά αποτελέσματα που δείχνουν τις λεπτομέρειες σχετικά με το τι συνέβη και ποιες ενέργειες μπορείτε να ακολουθήσετε για να κάνετε αλλαγές (εάν χρειάζονται αλλαγές).</span><span class="sxs-lookup"><span data-stu-id="6c6c2-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="6c6c2-108">**Βήματα για την αντιμετώπιση προβλημάτων εισόδου**</span><span class="sxs-lookup"><span data-stu-id="6c6c2-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="6c6c2-109">Μεταβείτε στη σελίδα εισόδου του Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="6c6c2-110">Φιλτράρισμα εισόδου ανά χρήστη, χρονική περιοχή, εφαρμογή, κατάσταση, εφαρμογή προγράμματος-πελάτη και ούτω καθεξής.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="6c6c2-111">Επιλέξτε ένα συμβάν εισόδου και προβάλετε την καρτέλα "πρόσβαση υπό όρους" για να δείτε ποιες πολιτικές έχουν αξιολογηθεί.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="6c6c2-112">Κάντε κλικ στη γραμμή μιας πολιτικής για να δείτε τις λεπτομέρειες της πολιτικής και να καταλάβετε γιατί εφαρμόστηκε.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="6c6c2-113">**Εργαλεία για την αντιμετώπιση μιας πολιτικής πρόσβασης υπό όρους**</span><span class="sxs-lookup"><span data-stu-id="6c6c2-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="6c6c2-114">Η λειτουργία "μόνο αναφορά" σάς επιτρέπει να αξιολογείτε μια πολιτική χωρίς να επηρεάζονται οι χρήστες.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="6c6c2-115">Το εργαλείο what-if σάς επιτρέπει να προσομοιώσετε συμβάντα εισόδου και να δείτε ποιες πολιτικές ισχύουν.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="6c6c2-116">Το βιβλίο εργασίας "Insights and Reporting" εμφανίζει τις επιπτώσεις σε πραγματικό χρόνο κάθε πολιτικής.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="6c6c2-117">**Πολιτικές προστασίας γραμμής βάσης**</span><span class="sxs-lookup"><span data-stu-id="6c6c2-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="6c6c2-118">Οι πολιτικές προστασίας γραμμής βάσης έχουν καταργηθεί.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="6c6c2-119">Δεν εφαρμόζονται πλέον και σύντομα θα καταργηθούν από την πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="6c6c2-120">Συνιστούμε να ενεργοποιήσετε τις [προεπιλογές ασφαλείας](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="6c6c2-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="6c6c2-121">Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="6c6c2-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="6c6c2-122">[Βέλτιστες πρακτικές για την υπό όρους πρόσβαση στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Συνθήκες στην πρόσβαση](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 υπό όρους [Στοιχεία ελέγχου σε πρόσβαση](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 υπό όρους [Θέσεις στην πρόσβαση υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="6c6c2-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
