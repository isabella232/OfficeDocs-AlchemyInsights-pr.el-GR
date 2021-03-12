---
title: Αντιμετώπιση προβλημάτων εγκατάστασης MDATP σε Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746304"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="35f2f-102">Αντιμετώπιση προβλημάτων εγκατάστασης MDATP σε Mac</span><span class="sxs-lookup"><span data-stu-id="35f2f-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="35f2f-103">Εάν αποτύχει η μη αυτόματη εγκατάσταση, **η σελίδα** "Σύνοψη" του οδηγού εγκατάστασης εμφανίζει το ακόλουθο σφάλμα:</span><span class="sxs-lookup"><span data-stu-id="35f2f-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="35f2f-104">"Παρουσιάστηκε σφάλμα κατά την εγκατάσταση.</span><span class="sxs-lookup"><span data-stu-id="35f2f-104">"An error occurred during installation.</span></span> <span data-ttu-id="35f2f-105">Το πρόγραμμα εγκατάστασης αντιμετώπισε ένα σφάλμα που προκάλεσε την αποτυχία της εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="35f2f-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="35f2f-106">Επικοινωνήστε με τον κατασκευαστή του λογισμικού για βοήθεια."</span><span class="sxs-lookup"><span data-stu-id="35f2f-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="35f2f-107">Για αναπτύξεις MDM, η σελίδα εμφανίζει επίσης μια γενική αποτυχία εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="35f2f-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="35f2f-108">Παρόλο που δεν εμφανίζονται ακριβή σφάλματα στους τελικούς χρήστες, διατηρείμε ένα αρχείο καταγραφής με την πρόοδο της εγκατάστασης, στο **/Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="35f2f-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="35f2f-109">Κάθε περίοδος λειτουργίας εγκατάστασης προσαρτάται σε αυτό το αρχείο καταγραφής.</span><span class="sxs-lookup"><span data-stu-id="35f2f-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="35f2f-110">Για να κάνετε έξοδο μόνο στην τελευταία περίοδο λειτουργίας εγκατάστασης, χρησιμοποιήστε `sed` το .</span><span class="sxs-lookup"><span data-stu-id="35f2f-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="35f2f-111">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων εγκατάστασης για [το Microsoft Defender ATP για Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="35f2f-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
