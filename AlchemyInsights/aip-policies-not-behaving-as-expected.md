---
title: 'AIP: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493024"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="9b250-102">AIP: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="9b250-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="9b250-103">Προστασία πληροφοριών Azure: Οι πολιτικές δεν συμπεριφέρονται όπως αναμένεται, ανατρέξτε στα παρακάτω για τις προτεινόμενες οδηγίες για διάφορα ζητήματα πολιτικής:</span><span class="sxs-lookup"><span data-stu-id="9b250-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="9b250-104">Εάν αντιμετωπίζετε προβλήματα με οπτικές σημάνσεις, ανατρέξτε [στο θέμα Όταν εφαρμόζονται οπτικές σημάνσεις](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="9b250-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="9b250-105">Εάν αντιμετωπίζετε προβλήματα με την αυτόματη επισήμανση, ανατρέξτε στο [θέμα Τρόπος ρύθμισης παραμέτρων συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="9b250-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="9b250-106">Εάν αντιμετωπίζετε προβλήματα με την προστασία εγγενούς/pfile, εξετάστε [τη ρύθμιση παραμέτρων API αρχείου](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="9b250-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="9b250-107">Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί σωστά: [Πώς να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="9b250-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="9b250-108">Εάν η αυτόματη επισήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: [ρυθμίσεις μητρώου IRM για ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="9b250-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="9b250-109">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής υπολογιστών-πελατών προστασίας πληροφοριών Azure και επισυνάψτε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το δελτίο.</span><span class="sxs-lookup"><span data-stu-id="9b250-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="9b250-110">Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="9b250-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="9b250-111">Κάντε κλικ στην επιλογή **Προστασία/Ευαισθησία**  >  **Βοήθεια και ανατροφοδότηση**.</span><span class="sxs-lookup"><span data-stu-id="9b250-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="9b250-112">Κάντε κλικ στην επιλογή **Εξαγωγή αρχείων καταγραφής**.</span><span class="sxs-lookup"><span data-stu-id="9b250-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="9b250-113">Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή τοποθεσίας σας και επισυνάψτε τα σε αυτήν την αίτηση υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="9b250-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="9b250-114">Πρόσθετοι πόροι:</span><span class="sxs-lookup"><span data-stu-id="9b250-114">Additional resources:</span></span>

- [<span data-ttu-id="9b250-115">Τρόπος ρύθμισης παραμέτρων ετικέτας για οπτικές σημάνσεις για προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="9b250-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="9b250-116">Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="9b250-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9b250-117">Χρήση ετικετών ευαισθησίας σε εφαρμογές του Office</span><span class="sxs-lookup"><span data-stu-id="9b250-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

