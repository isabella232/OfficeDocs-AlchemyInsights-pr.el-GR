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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694151"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="980fd-102">Επιδιόρθωση κανόνων μεταφοράς</span><span class="sxs-lookup"><span data-stu-id="980fd-102">Fix transport rules</span></span>

<span data-ttu-id="980fd-103">Ένας προσαρμοσμένος κανόνας ροής αλληλογραφίας επηρέασε αυτό το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="980fd-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="980fd-104">Για να εξετάσετε τον ακριβή κανόνα, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="980fd-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="980fd-105">Στα αποτελέσματα υποβολής, στην περιοχή **Πρόσθετες πληροφορίες,** σημειώστε το **GUID** ή το **όνομα της πολιτικής.**</span><span class="sxs-lookup"><span data-stu-id="980fd-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="980fd-106">Εκκινεί το Κέλυφος διαχείρισης Exchange.</span><span class="sxs-lookup"><span data-stu-id="980fd-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="980fd-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Άνοιγμα κελύφους διαχείρισης Exchange".](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="980fd-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="980fd-108">Εκτελέστε αυτή την εντολή (χρησιμοποιώντας το GUID από την υποβολή  **σας): Get-TransportRule -identity "GUID" | fl \* Περιγραφή**\*</span><span class="sxs-lookup"><span data-stu-id="980fd-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="980fd-109">Ελέγξτε την περιγραφή για να δείτε τις ρυθμισμένες συνθήκες που επηρέασαν το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="980fd-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="980fd-110">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="980fd-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
