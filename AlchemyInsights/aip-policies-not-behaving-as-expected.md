---
title: 'AIP: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663189"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="00930-102">AIP: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται</span><span class="sxs-lookup"><span data-stu-id="00930-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="00930-103">Προστασία πληροφοριών Azure: πολιτικές που δεν συμπεριφέρονται όπως αναμένεται, ανατρέξτε στα παρακάτω για τις προτεινόμενες οδηγίες για διάφορα θέματα πολιτικής:</span><span class="sxs-lookup"><span data-stu-id="00930-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="00930-104">Εάν αντιμετωπίζετε προβλήματα με οπτικές σημάνσεις, ανατρέξτε στο θέμα [πότε εφαρμόζονται οπτικές σημάνσεις](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="00930-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="00930-105">Εάν αντιμετωπίζετε προβλήματα με την αυτόματη σήμανση, εξετάστε τον τρόπο με τον οποίο μπορείτε [να ρυθμίσετε τις παραμέτρους για την αυτόματη και συνιστώμενη ταξινόμηση για την προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) και [Τι αναζητούν οι ευαίσθητοι τύποι πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="00930-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="00930-106">Εάν αντιμετωπίζετε προβλήματα με την εγγενή/Pfile προστασία, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων API αρχείου](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="00930-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="00930-107">Βεβαιωθείτε ότι χρησιμοποιείτε πολιτικές εύρους που δεν έχουν ρυθμιστεί σωστά: [Πώς μπορείτε να ρυθμίσετε τις παραμέτρους της πολιτικής προστασίας πληροφοριών Azure για συγκεκριμένους χρήστες χρησιμοποιώντας πολιτικές εύρους](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="00930-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="00930-108">Εάν η αυτόματη σήμανση δεν λειτουργεί για το Outlook κατά την επισύναψη ενός εγγράφου με ετικέτα, βεβαιωθείτε ότι το DRMEncryptProperty δεν έχει οριστεί όπως περιγράφεται εδώ: [ρυθμίσεις μητρώου IRM για την ασφάλεια](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="00930-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="00930-109">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, παρακαλούμε να συλλέξετε αρχεία καταγραφής προγράμματος-πελάτη προστασίας πληροφοριών Azure και να επισυνάψετε τα αρχεία καταγραφής που έχουν εξαχθεί σε αυτό το εισιτήριο.</span><span class="sxs-lookup"><span data-stu-id="00930-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="00930-110">Ανοίξτε ένα έγγραφο του Office ή δημιουργήστε ένα νέο μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook.</span><span class="sxs-lookup"><span data-stu-id="00930-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="00930-111">Κάντε κλικ στην επιλογή **προστασία/**  >  **Βοήθεια με ευαισθησία και σχόλια**.</span><span class="sxs-lookup"><span data-stu-id="00930-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="00930-112">Κάντε κλικ στην επιλογή **εξαγωγή αρχείων καταγραφής**.</span><span class="sxs-lookup"><span data-stu-id="00930-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="00930-113">Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή της τοποθεσίας σας και επισυνάψτε τα σε αυτή την αίτηση εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="00930-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="00930-114">Πρόσθετοι πόροι:</span><span class="sxs-lookup"><span data-stu-id="00930-114">Additional resources:</span></span>

- [<span data-ttu-id="00930-115">Πώς μπορείτε να ρυθμίσετε τις παραμέτρους μιας ετικέτας για οπτικές σημάνσεις για την προστασία πληροφοριών του Azure</span><span class="sxs-lookup"><span data-stu-id="00930-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="00930-116">Αναθεώρηση τεκμηρίωσης προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="00930-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="00930-117">Χρήση ετικετών ευαισθησίας στις εφαρμογές του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="00930-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

