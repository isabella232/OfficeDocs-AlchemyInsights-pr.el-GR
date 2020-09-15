---
title: Εγκατάσταση του Office σε διακομιστή τερματικού-χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663117"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d84e7-102">Εγκατάσταση του Office σε διακομιστή τερματικού</span><span class="sxs-lookup"><span data-stu-id="d84e7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d84e7-103">Για την ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις σε Windows Server με χρήση υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), παλαιότερα επώνυμων υπηρεσιών Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="d84e7-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d84e7-104">Πρέπει να έχετε μια συνδρομή Microsoft 365 που περιλαμβάνει εφαρμογές του Microsoft 365 για επιχειρήσεις, όπως το Office 365 Enterprise E3 ή το Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d84e7-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="d84e7-105">Οι εφαρμογές Microsoft 365 για επιχειρήσεις και Microsoft 365 για προγράμματα Premium για επιχειρήσεις δεν περιλαμβάνουν εφαρμογές του Microsoft 365 για επιχειρήσεις.</span><span class="sxs-lookup"><span data-stu-id="d84e7-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="d84e7-106">Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d84e7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="d84e7-107">Εάν θέλετε να εγκαταστήσετε τις εφαρμογές του Microsoft 365 για επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, χρησιμοποιήστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="d84e7-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="d84e7-108">Μπορείτε επίσης να κάνετε λήψη και να εκτελέσετε τον [Βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις εφαρμογές Microsoft 365 για επιχειρήσεις σε λειτουργία ενεργοποίησης κοινόχρηστων υπολογιστών.</span><span class="sxs-lookup"><span data-stu-id="d84e7-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="d84e7-109">Επιλέξτε τη συνδρομή Microsoft 365 που έχετε.</span><span class="sxs-lookup"><span data-stu-id="d84e7-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="d84e7-110">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="d84e7-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="d84e7-111">Εάν είναι απαραίτητο, μεταβείτε σε μια διαφορετική συνδρομή του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d84e7-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="d84e7-112">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="d84e7-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="d84e7-113">Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές του Microsoft 365, καταργήστε την εγκατάστασή του.</span><span class="sxs-lookup"><span data-stu-id="d84e7-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="d84e7-114">Για παράδειγμα, μεταβαίνοντας στον πίνακα ελέγχου, \> καταργήστε την εγκατάσταση ενός προγράμματος.</span><span class="sxs-lookup"><span data-stu-id="d84e7-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="d84e7-115">Καταργήστε την εγκατάσταση χρησιμοποιώντας [το βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν αντιμετωπίζετε προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="d84e7-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="d84e7-116">Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή σας και [Εγκαταστήστε τις εφαρμογές microsoft 365 για επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d84e7-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="d84e7-117">Μετά την εγκατάσταση του Office, ***Μην ανοίγετε ή εισέρχεστε*** σε οποιαδήποτε εφαρμογή του Office.</span><span class="sxs-lookup"><span data-stu-id="d84e7-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="d84e7-118">Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή, επεξεργαζόμενοι το μητρώο ακολουθώντας τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="d84e7-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="d84e7-119">Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση.</span><span class="sxs-lookup"><span data-stu-id="d84e7-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="d84e7-120">Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.</span><span class="sxs-lookup"><span data-stu-id="d84e7-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="d84e7-121">Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="d84e7-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="d84e7-122">Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς του **SharedComputerLicensing** με μια ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d84e7-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="d84e7-123">Στο διακομιστή RDS, ***Πραγματοποιήστε είσοδο ως τελικός χρήστης*** και [Επαληθεύστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για τις εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d84e7-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="d84e7-124">Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [ανάπτυξη εφαρμογών Microsoft 365 για επιχειρήσεις με τη χρήση υπηρεσιών απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d84e7-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="d84e7-125">Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση του κοινόχρηστου υπολογιστή, ανατρέξτε στο [θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για τις εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d84e7-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  