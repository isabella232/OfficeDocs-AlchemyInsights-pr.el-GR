---
title: Αντιμετώπιση προβλημάτων με Office 365 για προχωρημένους απειλή προστασίας (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030976"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="a7fa2-102">Αντιμετώπιση προβλημάτων σχετικά με το Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="a7fa2-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="a7fa2-103">**Παρατηρήστε καθυστερήσεις παράδοση μηνυμάτων ηλεκτρονικού ταχυδρομείου**;</span><span class="sxs-lookup"><span data-stu-id="a7fa2-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="a7fa2-104">Δοκιμάστε να χρησιμοποιήσετε την επιλογή παράδοσης δυναμικό για τις πολιτικές σας ATP ασφαλή συνημμένα.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="a7fa2-105">Την αποφυγή καθυστερήσεων παράδοσης μηνυμάτων ηλεκτρονικού ταχυδρομείου κατά την προστασία των παραληπτών από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="a7fa2-106">**Θέλετε να την αναφορά εσφαλμένες θετικές αναγνωρίσεις ή ψευδώς αρνητικών**;</span><span class="sxs-lookup"><span data-stu-id="a7fa2-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="a7fa2-107">Χρησιμοποιήστε αυτήν τη σύνδεση για να υποβάλετε το αρχείο σας για ανάλυση:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="a7fa2-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="a7fa2-108">**Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία ATP ασφαλείς συνδέσεις για μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ άτομα στον οργανισμό σας**;</span><span class="sxs-lookup"><span data-stu-id="a7fa2-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="a7fa2-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="a7fa2-109">Follow these steps:</span></span>
    1. <span data-ttu-id="a7fa2-110">Μεταβείτε στην https://protection.office.com, και να εισέλθετε.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="a7fa2-111">Μεταβείτε στη **Διαχείριση της απειλής** > **πολιτική** > **Ασφαλείς συνδέσεις**.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="a7fa2-112">Σύμφωνα με τις **πολιτικές που εφαρμόζονται σε συγκεκριμένους παραλήπτες**, επεξεργαστείτε (ή να προσθέσετε) μια πολιτική.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="a7fa2-113">Επιλέξτε **εφαρμογή ασφαλείς συνδέσεις σε μηνύματα που αποστέλλονται μέσα στην εταιρεία**.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="a7fa2-114">Αποθηκεύστε την πολιτική σας και περιμένετε περίπου 30 λεπτά για να λειτουργούν με τους τρόπο μέσω του κέντρου δεδομένων σας αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="a7fa2-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="a7fa2-115">Για να λάβετε περισσότερη βοήθεια σχετικά με ATP, ανατρέξτε στο θέμα [Προστασίας για προχωρημένους απειλή του Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="a7fa2-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>