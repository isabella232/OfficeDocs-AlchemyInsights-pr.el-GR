---
title: Αντιμετώπιση προβλημάτων με την Προστασία από απειλές για προχωρημένους (ATP) του Office 365 για προχωρημένους
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766745"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="b5578-102">Αντιμετώπιση προβλημάτων με το ATP του Office 365</span><span class="sxs-lookup"><span data-stu-id="b5578-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="b5578-103">**Ειδοποιήσεις καθυστερήσεις με την παράδοση μηνυμάτων ηλεκτρονικού ταχυδρομείου;**</span><span class="sxs-lookup"><span data-stu-id="b5578-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="b5578-104">Δοκιμάστε να χρησιμοποιήσετε την επιλογή δυναμικής παράδοσης για τις πολιτικές "Ασφαλή συνημμένα ATP".</span><span class="sxs-lookup"><span data-stu-id="b5578-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="b5578-105">Αυτό θα αποφύγει τις καθυστερήσεις παράδοσης μηνυμάτων ηλεκτρονικού ταχυδρομείου προστατεύοντας τους παραλήπτες από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="b5578-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="b5578-106">**Θέλετε να αναφέρετε ψευδώς θετικά ή ψευδώς αρνητικά;**</span><span class="sxs-lookup"><span data-stu-id="b5578-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="b5578-107">Χρησιμοποιήστε αυτόν το σύνδεσμο για να υποβάλετε το αρχείο σας για ανάλυση:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="b5578-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="b5578-108">**Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία atp safe links για μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ ατόμων στον οργανισμό σας;**</span><span class="sxs-lookup"><span data-stu-id="b5578-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="b5578-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="b5578-109">Follow these steps:</span></span>
    1. <span data-ttu-id="b5578-110">Μεταβείτε https://protection.office.comστο και συνδεθείτε.</span><span class="sxs-lookup"><span data-stu-id="b5578-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="b5578-111">Μεταβείτε στην επιλογή**Ασφαλείς συνδέσεις\*\*\*\*πολιτικής** >  **διαχείρισης** > απειλών .</span><span class="sxs-lookup"><span data-stu-id="b5578-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="b5578-112">Στην περιοχή **Πολιτικές που ισχύουν για συγκεκριμένους παραλήπτες**, επεξεργαστείτε (ή προσθέστε) μια πολιτική.</span><span class="sxs-lookup"><span data-stu-id="b5578-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="b5578-113">Επιλέξτε **Εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός του οργανισμού**.</span><span class="sxs-lookup"><span data-stu-id="b5578-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="b5578-114">Αποθηκεύστε την πολιτική σας και επιτρέψτε σε περίπου 30 λεπτά να λειτουργούν οι αλλαγές τους μέσω του κέντρου δεδομένων σας.</span><span class="sxs-lookup"><span data-stu-id="b5578-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="b5578-115">Για να λάβετε περισσότερη βοήθεια σχετικά με την ATP, [ανατρέξτε στο θέμα Προστασία από απειλές για προχωρημένους του Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="b5578-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>