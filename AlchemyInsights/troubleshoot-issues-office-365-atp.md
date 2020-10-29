---
title: Αντιμετώπιση προβλημάτων με το Microsoft Defender για το Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801407"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="b94b5-102">Αντιμετώπιση προβλημάτων με το Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="b94b5-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="b94b5-103">**Καθυστερήσεις ειδοποίησης με την παράδοση μηνυμάτων ηλεκτρονικού ταχυδρομείου** ;</span><span class="sxs-lookup"><span data-stu-id="b94b5-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="b94b5-104">Δοκιμάστε να χρησιμοποιήσετε την επιλογή δυναμικής παράδοσης για τις πολιτικές των ασφαλών συνημμένων ATP.</span><span class="sxs-lookup"><span data-stu-id="b94b5-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="b94b5-105">Αυτό θα αποτρέψει καθυστερήσεις παράδοσης μηνυμάτων ηλεκτρονικού ταχυδρομείου ενώ προστατεύει τους παραλήπτες από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="b94b5-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="b94b5-106">**Θέλετε να αναφέρετε ψευδώς θετικά ή ψευδή αρνητικά** ;</span><span class="sxs-lookup"><span data-stu-id="b94b5-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="b94b5-107">Χρησιμοποιήστε αυτήν τη σύνδεση για να υποβάλετε το αρχείο σας για ανάλυση: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="b94b5-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="b94b5-108">Γνωρίζατε **ότι μπορείτε να ενεργοποιήσετε την προστασία των ασφαλών συνδέσεων ATP για μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ ατόμων στην εταιρεία σας** ;</span><span class="sxs-lookup"><span data-stu-id="b94b5-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="b94b5-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="b94b5-109">Follow these steps:</span></span>
    1. <span data-ttu-id="b94b5-110">Μεταβείτε στην https://protection.office.com και πραγματοποιήστε είσοδο.</span><span class="sxs-lookup"><span data-stu-id="b94b5-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="b94b5-111">Μεταβείτε στις **Threat management**  >  **Policy**  >  **ασφαλείς συνδέσεις** της πολιτικής διαχείρισης απειλών.</span><span class="sxs-lookup"><span data-stu-id="b94b5-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="b94b5-112">Στην περιοχή **πολιτικές που ισχύουν για συγκεκριμένους παραλήπτες** , επεξεργαστείτε (ή προσθέστε) μια πολιτική.</span><span class="sxs-lookup"><span data-stu-id="b94b5-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="b94b5-113">Επιλέξτε **εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός του οργανισμού** .</span><span class="sxs-lookup"><span data-stu-id="b94b5-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="b94b5-114">Αποθηκεύστε την πολιτική σας και επιτρέψτε περίπου 30 λεπτά για να λειτουργήσουν οι αλλαγές σας μέσω του Datacenter.</span><span class="sxs-lookup"><span data-stu-id="b94b5-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="b94b5-115">Για να λάβετε περισσότερη βοήθεια με το ATP, ανατρέξτε στο θέμα [Microsoft Defender για το Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="b94b5-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>