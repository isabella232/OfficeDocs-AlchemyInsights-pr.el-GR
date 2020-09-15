---
title: Αντιμετώπιση προβλημάτων του Office 365 προηγμένη προστασία από απειλές
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658914"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="e8962-102">Αντιμετώπιση προβλημάτων του Office 365 προηγμένη προστασία από απειλές</span><span class="sxs-lookup"><span data-stu-id="e8962-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="e8962-103">Παρατηρείτε καθυστερήσεις στην παράδοση μηνυμάτων;</span><span class="sxs-lookup"><span data-stu-id="e8962-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="e8962-104">Χρησιμοποιήστε την επιλογή [δυναμικής παράδοσης](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) στην πολιτική των ασφαλών συνημμένων ATP.</span><span class="sxs-lookup"><span data-stu-id="e8962-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="e8962-105">Αυτό θα βοηθήσει στην αποφυγή των καθυστερήσεων των μηνυμάτων κατά την προστασία των παραληπτών από κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="e8962-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e8962-106">Θέλετε να αναφέρετε ψευδώς θετικά ή ψευδή αρνητικά στοιχεία στη Microsoft;</span><span class="sxs-lookup"><span data-stu-id="e8962-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="e8962-107">Χρησιμοποιήστε αυτήν τη [σύνδεση](https://www.microsoft.com/wdsi/filesubmission/) για να υποβάλετε αρχεία για ανάλυση.</span><span class="sxs-lookup"><span data-stu-id="e8962-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="e8962-108">Γνωρίζατε ότι μπορείτε να ενεργοποιήσετε την προστασία ασφαλών συνδέσεων για εσωτερικό ηλεκτρονικό ταχυδρομείο που έχει αποσταλεί μεταξύ παραληπτών εντός της εταιρείας σας;</span><span class="sxs-lookup"><span data-stu-id="e8962-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="e8962-109">Ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="e8962-109">Follow these steps:</span></span>

  1. <span data-ttu-id="e8962-110">Μεταβείτε [https://protection.office.com](https://protection.office.com) και πραγματοποιήστε είσοδο με έναν καθολικό διαχειριστή ή έναν λογαριασμό διαχειριστή ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="e8962-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e8962-111">Στο αριστερό παράθυρο περιήγησης, στην περιοχή **διαχείριση απειλών**, επιλέξτε **Policy** \> **ασφαλείς συνδέσεις**πολιτικής.</span><span class="sxs-lookup"><span data-stu-id="e8962-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="e8962-112">Στις **πολιτικές που ισχύουν για ολόκληρη την** ενότητα του οργανισμού, επιλέξτε την πολιτική και κάντε κλικ στην επιλογή **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="e8962-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="e8962-113">Στην περιοχή **Ρυθμίσεις**, ενεργοποιήστε **την επιλογή εφαρμογή ασφαλών συνδέσεων σε μηνύματα που αποστέλλονται εντός της εταιρείας**.</span><span class="sxs-lookup"><span data-stu-id="e8962-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
