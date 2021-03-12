---
title: Παράδειγμα πολιτικής ασφαλούς συνημμένου του Microsoft Defender για Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745996"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="30203-102">Παράδειγμα πολιτικής ασφαλούς συνημμένου του Microsoft Defender για Office 365</span><span class="sxs-lookup"><span data-stu-id="30203-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="30203-103">Αυτές οι ρυθμίσεις ενεργοποιούν μια πολιτική που ονομάζεται *"Χωρίς* καθυστερήσεις" που παραδίδει μηνύματα αμέσως και, στη συνέχεια, επανασυνδέει τα συνημμένα μετά τη σάρωση:</span><span class="sxs-lookup"><span data-stu-id="30203-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="30203-104">**Όνομα:** Χωρίς καθυστερήσεις</span><span class="sxs-lookup"><span data-stu-id="30203-104">**Name**: No delays</span></span>
- <span data-ttu-id="30203-105">**Περιγραφή:** Παραδίδει αμέσως μηνύματα και επανασυνδέει τα συνημμένα μετά τη σάρωση.</span><span class="sxs-lookup"><span data-stu-id="30203-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="30203-106">**Απόκριση:** Ενεργοποιήστε την **επιλογή δυναμικής παράδοσης.**</span><span class="sxs-lookup"><span data-stu-id="30203-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="30203-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Δυναμική παράδοση στις πολιτικές ασφαλών συνημμένων.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="30203-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="30203-108">**Ενότητα ανακατεύθυνσης** συνημμένου: Ενεργοποιήστε την επιλογή "Ενεργοποίηση ανακατεύθυνσης" **και,** στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του καθολικού διαχειριστή του Microsoft 365, του διαχειριστή ασφαλείας ή του αναλυτή ασφαλείας που θα ερευνήσει τα κακόβουλα συνημμένα.</span><span class="sxs-lookup"><span data-stu-id="30203-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="30203-109">**Ενότητα "Εφαρμόστηκε** σε": **Επιλέξτε τον τομέα παραλήπτη και,** στη συνέχεια, επιλέξτε τον τομέα σας.</span><span class="sxs-lookup"><span data-stu-id="30203-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="30203-110">Επιλέξτε **"Προσθήκη"** και, στη συνέχεια, **επιλέξτε OK.**</span><span class="sxs-lookup"><span data-stu-id="30203-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="30203-111">Όταν τελειώσετε, επιλέξτε **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="30203-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="30203-112">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Ασφαλή συνημμένα στο Microsoft Defender για Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="30203-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
