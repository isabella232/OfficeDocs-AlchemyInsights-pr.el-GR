---
title: Αντιμετώπιση προβλημάτων του Microsoft Defender για Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545268"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="67c4d-102">Αντιμετώπιση προβλημάτων του Microsoft Defender για Office 365</span><span class="sxs-lookup"><span data-stu-id="67c4d-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="67c4d-103">**Παρατηρήσατε καθυστερήσεις στην παράδοση μηνυμάτων;**</span><span class="sxs-lookup"><span data-stu-id="67c4d-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="67c4d-104">Χρησιμοποιήστε την [επιλογή δυναμικής παράδοσης](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) στον Microsoft Defender για Office 365 πολιτική ασφαλών συνημμένων.</span><span class="sxs-lookup"><span data-stu-id="67c4d-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="67c4d-105">Αυτό θα σας βοηθήσει να αποφύγετε καθυστερήσεις μηνυμάτων κατά την προστασία των παραληπτών από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="67c4d-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="67c4d-106">**Θέλετε να αναφέρετε ψευδή θετικά ή ψευδή αρνητικά στη Microsoft;**</span><span class="sxs-lookup"><span data-stu-id="67c4d-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="67c4d-107">Χρησιμοποιήστε [την Εξερεύνηση υποβολών.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="67c4d-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="67c4d-108">-\*\* Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία ασφαλών συνδέσεων για εσωτερικά μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται μεταξύ παραληπτών εντός του οργανισμού σας;\*\* Ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="67c4d-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="67c4d-109">Μεταβείτε [https://protection.office.com](https://protection.office.com) και πραγματοποιήστε είσοδο με έναν καθολικό διαχειριστή ή λογαριασμό διαχειριστή ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="67c4d-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="67c4d-110">Στο αριστερό παράθυρο περιήγησης στην περιοχή Διαχείριση **απειλών,** επιλέξτε **"Ασφαλείς** \> **συνδέσεις πολιτικής".**</span><span class="sxs-lookup"><span data-stu-id="67c4d-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="67c4d-111">Στις **πολιτικές που ισχύουν για ολόκληρη την ενότητα του οργανισμού,** επιλέξτε την πολιτική και κάντε κλικ στην επιλογή **"Επεξεργασία".**</span><span class="sxs-lookup"><span data-stu-id="67c4d-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="67c4d-112">Στην **Ρυθμίσεις , ενεργοποιήστε** την επιλογή **"Εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός του οργανισμού".**</span><span class="sxs-lookup"><span data-stu-id="67c4d-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
