---
title: Επιδιόρθωση κανόνων μεταφοράς
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746738"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="941d3-102">Επιδιόρθωση κανόνων μεταφοράς</span><span class="sxs-lookup"><span data-stu-id="941d3-102">Fix transport rules</span></span>

<span data-ttu-id="941d3-103">Ένας προσαρμοσμένος κανόνας ροής αλληλογραφίας επηρέασε αυτό το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="941d3-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="941d3-104">Για να ελέγξετε τον ακριβή κανόνα, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="941d3-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="941d3-105">Στα αποτελέσματα υποβολής, στην περιοχή **Πρόσθετες πληροφορίες,** σημειώστε το **GUID** ή **το όνομα πολιτικής.**</span><span class="sxs-lookup"><span data-stu-id="941d3-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="941d3-106">Εκκινεί το κέλυφος διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="941d3-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="941d3-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Άνοιγμα του κελύφους διαχείρισης του Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="941d3-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="941d3-108">Εκτελέστε αυτή την εντολή (χρησιμοποιώντας το GUID από την υποβολή σας):  **Get-TransportRule -identity "GUID" | fl \* Περιγραφή**\*</span><span class="sxs-lookup"><span data-stu-id="941d3-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="941d3-109">Εξετάστε την περιγραφή για να δείτε τις ρυθμισμένες συνθήκες που επηρέασαν το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="941d3-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="941d3-110">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="941d3-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
