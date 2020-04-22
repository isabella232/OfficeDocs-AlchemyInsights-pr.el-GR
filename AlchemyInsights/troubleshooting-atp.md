---
title: Αντιμετώπιση προβλημάτων προστασίας από απειλές για προχωρημένους του Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732402"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="4165a-102">Αντιμετώπιση προβλημάτων προστασίας από απειλές για προχωρημένους του Office 365</span><span class="sxs-lookup"><span data-stu-id="4165a-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="4165a-103">Παρατηρείτε καθυστερήσεις στην παράδοση μηνυμάτων;</span><span class="sxs-lookup"><span data-stu-id="4165a-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="4165a-104">Χρησιμοποιήστε την επιλογή [δυναμικής παράδοσης](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) στην πολιτική ασφαλούς συνημμένων ATP.</span><span class="sxs-lookup"><span data-stu-id="4165a-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="4165a-105">Αυτό θα βοηθήσει στην αποφυγή καθυστερήσεων μηνυμάτων κατά την προστασία των παραληπτών από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="4165a-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="4165a-106">Θέλετε να αναφέρετε ψευδώς θετικά ή ψευδώς αρνητικά στη Microsoft;</span><span class="sxs-lookup"><span data-stu-id="4165a-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="4165a-107">Χρησιμοποιήστε αυτήν τη [σύνδεση](https://www.microsoft.com/wdsi/filesubmission/) για να υποβάλετε αρχεία για ανάλυση.</span><span class="sxs-lookup"><span data-stu-id="4165a-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="4165a-108">Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία ασφαλών συνδέσεων για εσωτερικά μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ παραληπτών εντός του οργανισμού σας;</span><span class="sxs-lookup"><span data-stu-id="4165a-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="4165a-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="4165a-109">Follow these steps:</span></span>

  1. <span data-ttu-id="4165a-110">Μεταβείτε [https://protection.office.com](https://protection.office.com) και συνδεθείτε με έναν καθολικό λογαριασμό διαχειριστή ή διαχειριστή ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4165a-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="4165a-111">Στο αριστερό παράθυρο περιήγησης στην περιοχή **Διαχείριση απειλών**, επιλέξτε **Ασφαλείς συνδέσεις πολιτικής** \> **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="4165a-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="4165a-112">Στην **ενότητα Πολιτικές που ισχύουν για ολόκληρη την εταιρεία,** επιλέξτε την πολιτική και κάντε κλικ στην επιλογή **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="4165a-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="4165a-113">Στην περιοχή **Ρυθμίσεις**, **ενεργοποιήστε την επιλογή Εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός του οργανισμού**.</span><span class="sxs-lookup"><span data-stu-id="4165a-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
