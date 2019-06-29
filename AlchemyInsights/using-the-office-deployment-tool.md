---
title: Χρησιμοποιώντας το εργαλείο ανάπτυξης του Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365525"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="391d5-102">Χρησιμοποιώντας το εργαλείο ανάπτυξης του Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="391d5-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="391d5-103">Μπορείτε να χρησιμοποιήσετε το Office ανάπτυξης Tool (ODT) για την ανάπτυξη του Office 365 εκδόσεις του Office.</span><span class="sxs-lookup"><span data-stu-id="391d5-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="391d5-104">Το εργαλείο ανάπτυξης του Office (setup.exe) εκτελείται από τη γραμμή εντολών και χρησιμοποιεί το αρχείο ρύθμισης παραμέτρων XML για να προσδιορίσετε ποιες ρυθμίσεις πρέπει να εφαρμόζονται κατά την ανάπτυξη του Office.</span><span class="sxs-lookup"><span data-stu-id="391d5-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="391d5-105">Λήψη της τελευταίας έκδοσης του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="391d5-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="391d5-106">Χρησιμοποιήστε το [Εργαλείο προσαρμογής του Office (OCT)](https://config.office.com) για να επιλέξετε τις προτιμήσεις σας ανάπτυξης και να δημιουργήσετε αρχείο ρύθμισης παραμέτρων XML.</span><span class="sxs-lookup"><span data-stu-id="391d5-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="391d5-107">Εξαγάγετε το αρχείο ρύθμισης παραμέτρων και τοποθετήστε το τοπικά στον ίδιο φάκελο όπου βρίσκεται το setup.exe.</span><span class="sxs-lookup"><span data-stu-id="391d5-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="391d5-108">**Σημείωση:** Εγκατάσταση του Office που συνήθως παρουσιάζονται ζητήματα οφείλεται σε εσφαλμένες ρυθμίσεις ή αρχεία ρύθμισης παραμέτρων malformatted.</span><span class="sxs-lookup"><span data-stu-id="391d5-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="391d5-109">Για να αποφύγετε αυτά τα ζητήματα, συνιστάται να χρησιμοποιήσετε το εργαλείο προσαρμογής του Office για να δημιουργήσετε το αρχείο ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="391d5-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="391d5-110">Μπορείτε επίσης να εισαγάγετε υπάρχοντα αρχεία ρύθμισης παραμέτρων στο εργαλείο προσαρμογής του Office.</span><span class="sxs-lookup"><span data-stu-id="391d5-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="391d5-111">Από μια γραμμή εντολών με αναβαθμισμένα δικαιώματα, μεταβείτε στη θέση όπου βρίσκεται το setup.exe και εκτελέσετε το εργαλείο ανάπτυξης του Office σε λειτουργία λήψης και καθορίστε το αρχείο ρύθμισης παραμέτρων που μόλις αποθηκεύσατε.</span><span class="sxs-lookup"><span data-stu-id="391d5-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="391d5-112">Σε αυτό το παράδειγμα, το αρχείο ρύθμισης παραμέτρων ονομάζεται Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="391d5-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="391d5-113">Εκτελέστε το εργαλείο ανάπτυξης του Office σε λειτουργία ρύθμισης παραμέτρων και καθορίστε το αρχείο ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="391d5-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="391d5-114">**Σημείωση:** Πρέπει να εκτελέσετε αυτό το βήμα από τον υπολογιστή-πελάτη, στην οποία θέλετε να εγκαταστήσετε το Office και θα πρέπει να έχετε δικαιώματα τοπικού διαχειριστή σε αυτόν τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="391d5-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="391d5-115">Για να μάθετε περισσότερα σχετικά με τη χρήση της εργαλείο ανάπτυξης του Office για το Office 365 ProPlus σενάρια ανάπτυξης, ανατρέξτε στην ενότητα [Επισκόπηση του εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="391d5-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="391d5-116">Για περισσότερες λεπτομέρειες σχετικά με τον τρόπο για να χρησιμοποιήσετε το εργαλείο προσαρμογής του Office, ανατρέξτε στο θέμα [Επισκόπηση της εργαλείο προσαρμογής του Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="391d5-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
