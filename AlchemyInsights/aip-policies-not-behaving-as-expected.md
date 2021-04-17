---
title: 'AIP: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821627"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="23ed3-102">AIP: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="23ed3-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="23ed3-103">Προστασία πληροφοριών Azure: Οι πολιτικές δεν συμπεριφέρεται όπως αναμένεται, ανατρέξτε στα παρακάτω για προτεινόμενες οδηγίες για διάφορα ζητήματα πολιτικής:</span><span class="sxs-lookup"><span data-stu-id="23ed3-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="23ed3-104">Εάν αντιμετωπίζετε προβλήματα με τις οπτικές σημάνσεις, ελέγξτε [πότε εφαρμόζονται οπτικές σημάνσεις.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="23ed3-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="23ed3-105">Εάν αντιμετωπίζετε προβλήματα με την αυτόματη σήμανση, ανατρέξτε στο θέμα Πώς μπορείτε να ρυθμίσετε τις παραμέτρους των συνθηκών για την αυτόματη και συνιστώμενη ταξινόμηση για την Προστασία πληροφοριών [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και τι θα αναζητήσουν [οι τύποι ευαίσθητων πληροφοριών.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="23ed3-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="23ed3-106">Εάν αντιμετωπίζετε προβλήματα με την προστασία native/Pfile, εξετάστε τη ρύθμιση [παραμέτρων του File API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="23ed3-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="23ed3-107">Ελέγξτε εάν χρησιμοποιείτε πολιτικές εμβέλειας που δεν έχουν ρυθμιστεί σωστά: Πώς μπορείτε να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους [χρήστες, χρησιμοποιώντας πολιτικές εμβέλειας.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="23ed3-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="23ed3-108">Εάν η αυτόματη σήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: Ρυθμίσεις μητρώου [IRM για την ασφάλεια.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="23ed3-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="23ed3-109">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, συλλέξτε αρχεία καταγραφής προγράμματος-πελάτη προστασίας πληροφοριών Azure και επισυνάψτε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το δελτίο.</span><span class="sxs-lookup"><span data-stu-id="23ed3-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="23ed3-110">Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="23ed3-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="23ed3-111">Κάντε κλικ **στην επιλογή "Προστασία/Ευαισθησία**  >  **βοήθειας και σχολίων".**</span><span class="sxs-lookup"><span data-stu-id="23ed3-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="23ed3-112">Κάντε κλικ στην **επιλογή "Εξαγωγή αρχείων καταγραφής".**</span><span class="sxs-lookup"><span data-stu-id="23ed3-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="23ed3-113">Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή της τοποθεσίας σας και επισυνάψτε τα σε αυτή την αίτηση υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="23ed3-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="23ed3-114">Πρόσθετοι πόροι:</span><span class="sxs-lookup"><span data-stu-id="23ed3-114">Additional resources:</span></span>

- [<span data-ttu-id="23ed3-115">Τρόπος ρύθμισης παραμέτρων ετικέτας για οπτικές σημάνσεις για την Προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="23ed3-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="23ed3-116">Αναθεώρηση της τεκμηρίωσης προστασίας πληροφοριών azure</span><span class="sxs-lookup"><span data-stu-id="23ed3-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="23ed3-117">Χρήση ετικετών ευαισθησίας σε εφαρμογές του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="23ed3-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

