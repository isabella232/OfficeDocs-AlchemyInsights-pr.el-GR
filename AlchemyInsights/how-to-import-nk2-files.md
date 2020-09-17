---
title: Οδηγίες εισαγωγής-nk2-αρχεία
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780059"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="4aea0-102">Πώς μπορείτε να εισαγάγετε αρχεία. nk2</span><span class="sxs-lookup"><span data-stu-id="4aea0-102">How to import .nk2 files</span></span> 

<span data-ttu-id="4aea0-103">Όταν ξεκινάτε το Microsoft Outlook 2013, το Outlook 2016, το Outlook 2019 ή το Outlook για Microsoft 365 για πρώτη φορά, το cache του ψευδώνυμός σας (αποθηκευμένο στο αρχείο του *αρχείου. nk2*) εισάγεται σε ένα κρυφό μήνυμα στο προεπιλεγμένο χώρο αποθήκευσης μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="4aea0-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="4aea0-104">Για να εισαγάγετε αρχεία. nk2 στο Outlook 2013, το Outlook 2016, το Outlook 2019 ή το Outlook για Microsoft 365, βεβαιωθείτε ότι το αρχείο. nk2 βρίσκεται στον ακόλουθο φάκελο:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="4aea0-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="4aea0-105">**Σημείωση**: το αρχείο. nk2 πρέπει να έχει το ίδιο όνομα με το τρέχον προφίλ του Outlook 2013 ή του Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="4aea0-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="4aea0-106">Από προεπιλογή, το όνομα προφίλ είναι "Outlook".</span><span class="sxs-lookup"><span data-stu-id="4aea0-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="4aea0-107">Για να επιλέξετε το όνομα του προφίλ, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="4aea0-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="4aea0-108">Κάντε κλικ στην επιλογή **Έναρξη**και, στη συνέχεια, επιλέξτε **Πίνακας ελέγχου**.</span><span class="sxs-lookup"><span data-stu-id="4aea0-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="4aea0-109">Κάντε διπλό κλικ στην επιλογή **Αλληλογραφία**.</span><span class="sxs-lookup"><span data-stu-id="4aea0-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="4aea0-110">Στο παράθυρο διαλόγου Ρύθμιση αλληλογραφίας, επιλέξτε **Εμφάνιση προφίλ**.</span><span class="sxs-lookup"><span data-stu-id="4aea0-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="4aea0-111">Επιλέξτε **Έναρξη**  >  **εκτέλεσης**.</span><span class="sxs-lookup"><span data-stu-id="4aea0-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="4aea0-112">Στο πλαίσιο **Άνοιγμα** , πληκτρολογήστε *outlook.exe/importnk2*και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="4aea0-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="4aea0-113">Μετά την εισαγωγή του αρχείου. nk2, τα περιεχόμενα του αρχείου συγχωνεύονται στο υπάρχον cache ψευδώνυμων που είναι αποθηκευμένο στο γραμματοκιβώτιό σας.</span><span class="sxs-lookup"><span data-stu-id="4aea0-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="4aea0-114">**Σημείωση**: το αρχείο. nk2 μετονομάζεται με επέκταση ονόματος αρχείου. old την επόμενη φορά που θα ξεκινήσετε το Outlook 2013, το Outlook 2016, το Outlook 2019 ή το Outlook για Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4aea0-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="4aea0-115">Εάν θέλετε να επαναλάβετε την εισαγωγή του αρχείου. nk2, καταργήστε πρώτα την επέκταση ονόματος αρχείου. old.</span><span class="sxs-lookup"><span data-stu-id="4aea0-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="4aea0-116">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εισαγωγή ή αντιγραφή της λίστας αυτόματης καταχώρησης σε άλλον υπολογιστή](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="4aea0-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>