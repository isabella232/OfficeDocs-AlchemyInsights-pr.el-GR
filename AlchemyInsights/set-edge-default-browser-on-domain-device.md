---
title: Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε μια συσκευή που είναι συνδεδεμένος με τομέα
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491586"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="0c92d-102">Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε μια συσκευή που είναι συνδεδεμένος με τομέα</span><span class="sxs-lookup"><span data-stu-id="0c92d-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="0c92d-103">Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης:</span><span class="sxs-lookup"><span data-stu-id="0c92d-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="0c92d-104">[Δημιουργήστε ένα προεπιλεγμένο αρχείο ρύθμισης παραμέτρων συσχετίσεων](https://go.microsoft.com/fwlink/?linkid=2132437) και αποθηκεύστε το τοπικά ή σε ένα κοινόχρηστο στοιχείο δικτύου.</span><span class="sxs-lookup"><span data-stu-id="0c92d-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="0c92d-105">Ανοίξτε το πρόγραμμα επεξεργασίας πολιτικής ομάδας και, στη συνέχεια, μεταβείτε στην Εξερεύνηση αρχείων "Πρότυπα διαχείρισης ρύθμισης  >    >  **παραμέτρων υπολογιστή" των**  >  **Windows.**</span><span class="sxs-lookup"><span data-stu-id="0c92d-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="0c92d-106">Επιλέξτε **"Ορισμός προεπιλεγμένου αρχείου ρύθμισης παραμέτρων συσχετίσεων".**</span><span class="sxs-lookup"><span data-stu-id="0c92d-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="0c92d-107">Επιλέξτε **"Ρύθμιση πολιτικής" και,** στη συνέχεια, επιλέξτε **"Ενεργοποιημένο".**</span><span class="sxs-lookup"><span data-stu-id="0c92d-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="0c92d-108">Στην **περιοχή "Επιλογές",** πληκτρολογήστε τη θέση του προεπιλεγμένου αρχείου ρύθμισης παραμέτρων συσχετίσεων και, στη συνέχεια, **επιλέξτε OK.**</span><span class="sxs-lookup"><span data-stu-id="0c92d-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
