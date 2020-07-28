---
title: Πολλά αντικείμενα έχουν την ίδια διεύθυνση ηλεκτρονικού ταχυδρομείου με την ταυτότητα
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439195"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="588ef-102">Πολλά αντικείμενα έχουν την ίδια διεύθυνση ηλεκτρονικού ταχυδρομείου με την ταυτότητα</span><span class="sxs-lookup"><span data-stu-id="588ef-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="588ef-103">**Πολλά αντικείμενα**</span><span class="sxs-lookup"><span data-stu-id="588ef-103">**Multiple objects**</span></span>

<span data-ttu-id="588ef-104">Ένας από τους συνηθισμένους λόγους αυτού του σφάλματος είναι να μην μπορείτε να δρομολογήσατε σωστά μια αίτηση του Outlook Web Access παρουσία πολλών αντικειμένων που έχουν την ίδια διεύθυνση ηλεκτρονικού ταχυδρομείου με την ταυτότητα.</span><span class="sxs-lookup"><span data-stu-id="588ef-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="588ef-105">Για να βρείτε αυτά τα αντικείμενα, εκτελέστε τις ακόλουθες εντολές:</span><span class="sxs-lookup"><span data-stu-id="588ef-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="588ef-106">· Λήψη παραλήπτη<email address></span><span class="sxs-lookup"><span data-stu-id="588ef-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="588ef-107">· Λήψη χρήστη<email address></span><span class="sxs-lookup"><span data-stu-id="588ef-107">· Get-User <email address></span></span>

<span data-ttu-id="588ef-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="588ef-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="588ef-109">· Λήψη επαφής<email address></span><span class="sxs-lookup"><span data-stu-id="588ef-109">· Get-Contact <email address></span></span>

<span data-ttu-id="588ef-110">· Λήψη γραμματοκιβωτίου <email address> -Δημόσιος φάκελος</span><span class="sxs-lookup"><span data-stu-id="588ef-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="588ef-111">· Λήψη γραμματοκιβωτίου <email address> -Συμπερίληψη Πλαίσιο ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="588ef-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="588ef-112">· Λήψη γραμματοκιβωτίου <email address> -Ανενεργόςβωτοπώξωμα</span><span class="sxs-lookup"><span data-stu-id="588ef-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="588ef-113">Για να επιλύσετε το ζήτημα, καταργήστε πολλά αντικείμενα με την ίδια ταυτότητα ηλεκτρονικού ταχυδρομείου και βεβαιωθείτε ότι υπάρχει ένα μεμονωμένο αντικείμενο με τη συγκεκριμένη ταυτότητα ηλεκτρονικού ταχυδρομείου και ότι ο τύπος παραλήπτη του είναι UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="588ef-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="588ef-114">**Η ίδια διεύθυνση χρησιμοποιείται για γραμματοκιβώτια επιχειρήσεων και καταναλωτών**</span><span class="sxs-lookup"><span data-stu-id="588ef-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="588ef-115">Μια άλλη αιτία είναι όταν χρησιμοποιείται η ίδια διεύθυνση για γραμματοκιβώτια επιχειρήσεων και καταναλωτών.</span><span class="sxs-lookup"><span data-stu-id="588ef-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="588ef-116">Σε αυτήν την περίπτωση, ο χρήστης πρέπει να αλλάξει το ψευδώνυμο του κύριου καταναλωτή μέχρι cafe υποστηρίζει αυτό το σενάριο.</span><span class="sxs-lookup"><span data-stu-id="588ef-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="588ef-117">Πρόκειται για ένα μόνιμο σφάλμα που δεν φεύγει χωρίς παρέμβαση.</span><span class="sxs-lookup"><span data-stu-id="588ef-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="588ef-118">Για λεπτομέρειες, ανατρέξτε στο θέμα [Αλλαγή της διεύθυνσης ηλεκτρονικού ταχυδρομείου ή του αριθμού τηλεφώνου για το λογαριασμό Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="588ef-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>