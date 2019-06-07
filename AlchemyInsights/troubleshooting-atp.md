---
title: Αντιμετώπιση προβλημάτων του Office 365 για προχωρημένους απειλή προστασίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765097"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="0d5d7-102">Αντιμετώπιση προβλημάτων του Office 365 για προχωρημένους απειλή προστασίας</span><span class="sxs-lookup"><span data-stu-id="0d5d7-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="0d5d7-103">Παρατηρείτε καθυστερήσεις στην παράδοση μηνυμάτων;</span><span class="sxs-lookup"><span data-stu-id="0d5d7-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="0d5d7-104">Χρησιμοποιήστε την επιλογή [Παράδοσης δυναμική](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) στην πολιτική σας ATP ασφαλή συνημμένα.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="0d5d7-105">Αυτό θα βοηθήσει να αποφύγετε καθυστερήσεις μήνυμα ενώ ταυτόχρονα θα προστατεύει τους παραλήπτες από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="0d5d7-106">Θέλετε να αναφέρετε εσφαλμένες θετικές αναγνωρίσεις ή ψευδώς αρνητικών στη Microsoft;</span><span class="sxs-lookup"><span data-stu-id="0d5d7-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="0d5d7-107">Χρησιμοποιήστε αυτήν τη [σύνδεση](https://www.microsoft.com/wdsi/filesubmission/) για να υποβάλετε αρχεία για ανάλυση.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="0d5d7-108">Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία ασφαλείς συνδέσεις για εσωτερικό μήνυμα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ τους παραλήπτες εντός της εταιρείας σας;</span><span class="sxs-lookup"><span data-stu-id="0d5d7-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="0d5d7-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="0d5d7-109">Follow these steps:</span></span>

  1. <span data-ttu-id="0d5d7-110">Μεταβείτε στην [https://protection.office.com](https://protection.office.com) και πραγματοποιήστε είσοδο με ένα λογαριασμό διαχειριστή ασφαλείας ή καθολικός διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="0d5d7-111">Στο αριστερό παράθυρο περιήγησης στο πλαίσιο **διαχείρισης απειλή**, επιλέξτε **πολιτική** \> **Ασφαλείς συνδέσεις**.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="0d5d7-112">Στην ενότητα **πολιτικές που εφαρμόζονται σε ολόκληρο τον οργανισμό** , επιλέξτε την πολιτική και κάντε κλικ στο κουμπί **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="0d5d7-113">Στην περιοχή **Ρυθμίσεις**επιτρέπουν την **εφαρμογή ασφαλείς συνδέσεις σε μηνύματα που αποστέλλονται μέσα στην εταιρεία**.</span><span class="sxs-lookup"><span data-stu-id="0d5d7-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
