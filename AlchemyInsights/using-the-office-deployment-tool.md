---
title: Χρήση του εργαλείου ανάπτυξης του Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726248"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="086b1-102">Χρήση του εργαλείου ανάπτυξης του Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="086b1-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="086b1-103">Μπορείτε να χρησιμοποιήσετε το Εργαλείο ανάπτυξης του Office (ODT) για να αναπτύξετε εκδόσεις του Office 365 του Office.</span><span class="sxs-lookup"><span data-stu-id="086b1-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="086b1-104">Το Εργαλείο ανάπτυξης του Office (setup.exe) εκτελείται από τη γραμμή εντολών και χρησιμοποιεί ένα αρχείο XML ρύθμισης παραμέτρων για να καθορίσει ποιες ρυθμίσεις θα εφαρμοστούν κατά την ανάπτυξη του Office.</span><span class="sxs-lookup"><span data-stu-id="086b1-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="086b1-105">Κάντε λήψη της πιο πρόσφατης έκδοσης του Εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="086b1-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="086b1-106">Χρησιμοποιήστε το [Εργαλείο προσαρμογής του Office (OCT)](https://config.office.com) για να επιλέξετε τις προτιμήσεις ανάπτυξης και να δημιουργήσετε το αρχείο XML ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="086b1-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="086b1-107">Εξαγάγετε το αρχείο ρύθμισης παραμέτρων και τοποθετήστε το τοπικά στον ίδιο φάκελο όπου βρίσκεται το αρχείο setup.exe.</span><span class="sxs-lookup"><span data-stu-id="086b1-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="086b1-108">**Σημείωση:** Τα ζητήματα εγκατάστασης του Office συνήθως παρουσιάζονται λόγω αρχείων ρύθμισης παραμέτρων που δεν έχουν ρυθμιστεί σωστά ή έχουν διαμορφωθεί με βύνη.</span><span class="sxs-lookup"><span data-stu-id="086b1-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="086b1-109">Για να αποφύγετε τέτοια ζητήματα, συνιστάται να χρησιμοποιήσετε το εργαλείο προσαρμογής του Office για να δημιουργήσετε το αρχείο ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="086b1-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="086b1-110">Μπορείτε επίσης να εισαγάγετε υπάρχοντα αρχεία ρύθμισης παραμέτρων στο Εργαλείο προσαρμογής του Office.</span><span class="sxs-lookup"><span data-stu-id="086b1-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="086b1-111">Από μια γραμμή εντολών με αυξημένα επίπεδα, μεταβείτε στη θέση όπου βρίσκεται το αρχείο Setup.exe και εκτελέστε το Εργαλείο ανάπτυξης του Office σε λειτουργία λήψης και καθορίστε το αρχείο ρύθμισης παραμέτρων που μόλις αποθηκεύσατε.</span><span class="sxs-lookup"><span data-stu-id="086b1-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="086b1-112">Σε αυτό το παράδειγμα, το αρχείο ρύθμισης παραμέτρων ονομάζεται Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="086b1-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="086b1-113">Εκτελέστε το εργαλείο ανάπτυξης του Office σε λειτουργία ρύθμισης παραμέτρων και καθορίστε το αρχείο ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="086b1-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="086b1-114">**Σημείωση:** Πρέπει να εκτελέσετε αυτό το βήμα από τον υπολογιστή-πελάτη στον οποίο θέλετε να εγκαταστήσετε το Office και πρέπει να έχετε δικαιώματα τοπικού διαχειριστή σε αυτόν τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="086b1-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="086b1-115">Για να μάθετε περισσότερα σχετικά με τη χρήση του Εργαλείου ανάπτυξης του Office για τα σενάρια ανάπτυξης του Microsoft 365 Apps για επιχειρήσεις, [ανατρέξτε στο θέμα Επισκόπηση του Εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="086b1-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="086b1-116">Για περισσότερες λεπτομέρειες σχετικά με τον τρόπο χρήσης του εργαλείου προσαρμογής του Office, [ανατρέξτε στο θέμα Επισκόπηση του εργαλείου προσαρμογής του Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="086b1-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
