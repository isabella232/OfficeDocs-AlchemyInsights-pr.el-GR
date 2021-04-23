---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952228"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="298da-102">Πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange</span><span class="sxs-lookup"><span data-stu-id="298da-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="298da-103">Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="298da-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="298da-104">Εάν έχετε προβλήματα με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange που δεν ισχύουν για γραμματοκιβώτια ή στοιχεία που δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης, ελέγξτε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="298da-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="298da-105">**Ριζικές αιτίες:**</span><span class="sxs-lookup"><span data-stu-id="298da-105">**Root Causes:**</span></span>

- <span data-ttu-id="298da-106">**Ο Βοηθός διαχειριζόμενων** φακέλων δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="298da-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="298da-107">Ο Βοηθός διαχειριζόμενων φακέλων προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="298da-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="298da-108">**Λύση:** Εκτελέστε τον Βοηθό διαχείρισης φακέλων.</span><span class="sxs-lookup"><span data-stu-id="298da-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="298da-109">**Το RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="298da-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="298da-110">Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου.</span><span class="sxs-lookup"><span data-stu-id="298da-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="298da-111">**Λύση:** Ελέγξτε την κατάσταση της ρύθμισης διατήρησης και της ενημέρωσης, όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="298da-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="298da-112">Για λεπτομέρειες, ανατρέξτε στο [θέμα Διατήρηση γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="298da-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="298da-113">**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενων φακέλων δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="298da-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="298da-114">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέμα:</span><span class="sxs-lookup"><span data-stu-id="298da-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="298da-115">Ετικέτες διατήρησης και πολιτικές διατήρησης</span><span class="sxs-lookup"><span data-stu-id="298da-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="298da-116">[Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια ή προσθήκη](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="298da-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="298da-117">Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="298da-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
