---
title: Επιτάχυνση του SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931226"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ceb23-102">Επιτάχυνση του SharePoint online</span><span class="sxs-lookup"><span data-stu-id="ceb23-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="ceb23-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="ceb23-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ceb23-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="ceb23-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ceb23-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="ceb23-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ceb23-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="ceb23-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ceb23-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="ceb23-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ceb23-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="ceb23-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ceb23-109">**503 server είναι απασχολημένος σφάλμα**</span><span class="sxs-lookup"><span data-stu-id="ceb23-109">**503 server is busy error**</span></span>

<span data-ttu-id="ceb23-110">Οι χρήστες ενδέχεται να λάβουν ένα διακομιστή 503 είναι απασχολημένος σφάλμα κατά την προσπάθεια να περιηγηθείτε στο SharePoint ή τοποθεσίες του OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ceb23-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="ceb23-111">Αυτό το σφάλμα μπορεί να προκληθεί από τον περιορισμό της υπηρεσίας SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ceb23-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ceb23-112">Το SharePoint Online χρησιμοποιεί επιτάχυνση για να διατηρήσει τη βέλτιστη απόδοση και αξιοπιστία της υπηρεσίας SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ceb23-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ceb23-113">Ο περιορισμός περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (ανά δέσμη ενεργειών ή κώδικα) για να αποτραπεί η υπερβολική χρήση πόρων.</span><span class="sxs-lookup"><span data-stu-id="ceb23-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="ceb23-114">Για περισσότερες πληροφορίες σχετικά με τον περιορισμό, ανατρέξτε στο [θέμα Αποφύγετε τον περιορισμό ή τον αποκλεισμό στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ceb23-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="ceb23-115">Εάν πιστεύετε ότι αυτό το σφάλμα δεν σχετίζεται με τον περιορισμό, μπορείτε να ελέγξετε αν υπάρχει ενεργή συντήρηση που πραγματοποιείται στον μισθωτή σας μεταβαίνοντας στο [κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="ceb23-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="ceb23-116">Τέλος, βεβαιωθείτε ότι επισκέπτεστε τη σελίδα [Υπηρεσία Υγείας](https://portal.office.com/adminportal/home#/servicehealth) για να ελέγξετε για τυχόν συμβουλές / περιστατικά που μπορεί να συμβαίνουν.</span><span class="sxs-lookup"><span data-stu-id="ceb23-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

