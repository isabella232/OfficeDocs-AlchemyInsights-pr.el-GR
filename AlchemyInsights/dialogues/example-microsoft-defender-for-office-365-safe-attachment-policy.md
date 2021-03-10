---
title: Παράδειγμα πολιτικής ασφαλούς συνημμένου του Microsoft Defender για το Office 365
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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693825"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="a45dd-102">Παράδειγμα πολιτικής ασφαλούς συνημμένου του Microsoft Defender για το Office 365</span><span class="sxs-lookup"><span data-stu-id="a45dd-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="a45dd-103">Αυτές οι ρυθμίσεις ενεργοποιούν μια πολιτική που ονομάζεται *"Χωρίς* καθυστερήσεις" η οποία παραδίδει αμέσως τα μηνύματα και, στη συνέχεια, επανασυνδέει τα συνημμένα μετά τη σάρωση:</span><span class="sxs-lookup"><span data-stu-id="a45dd-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="a45dd-104">**Όνομα:** Καμία καθυστέρηση</span><span class="sxs-lookup"><span data-stu-id="a45dd-104">**Name**: No delays</span></span>
- <span data-ttu-id="a45dd-105">**Περιγραφή:** Παραδίδει μηνύματα αμέσως και επανασυνδέει τα συνημμένα μετά τη σάρωση.</span><span class="sxs-lookup"><span data-stu-id="a45dd-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="a45dd-106">**Απόκριση:** Ορίστε την **επιλογή δυναμικής παράδοσης.**</span><span class="sxs-lookup"><span data-stu-id="a45dd-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="a45dd-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Δυναμική παράδοση" στις πολιτικές ασφαλών συνημμένων.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="a45dd-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="a45dd-108">**Ενότητα** ανακατεύθυνσης συνημμένου: Ορίστε την επιλογή "Ενεργοποίηση ανακατεύθυνσης" **και,** στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του καθολικού διαχειριστή του Microsoft 365, του διαχειριστή ασφαλείας ή ενός αναλυτή ασφαλείας που θα διερευνήσει κακόβουλα συνημμένα.</span><span class="sxs-lookup"><span data-stu-id="a45dd-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="a45dd-109">**Ενότητα "Εφαρμογή** σε": Επιλέξτε **τον τομέα του παραλήπτη και,** στη συνέχεια, επιλέξτε τον τομέα σας.</span><span class="sxs-lookup"><span data-stu-id="a45dd-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="a45dd-110">Επιλέξτε **"Προσθήκη"** και, στη συνέχεια, **επιλέξτε "OK".**</span><span class="sxs-lookup"><span data-stu-id="a45dd-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="a45dd-111">Όταν τελειώσετε, επιλέξτε **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="a45dd-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="a45dd-112">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα "Ασφαλή συνημμένα" στον Microsoft Defender για το Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="a45dd-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
