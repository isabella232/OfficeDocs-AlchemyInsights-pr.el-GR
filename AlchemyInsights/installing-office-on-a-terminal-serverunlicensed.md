---
title: Εγκατάσταση γραφείου σε terminal server - Χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763217"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b482a-102">Εγκατάσταση του Office σε διακομιστή τερματικού</span><span class="sxs-lookup"><span data-stu-id="b482a-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b482a-103">Για την ανάπτυξη εφαρμογών microsoft 365 για επιχειρήσεις σε διακομιστή των Windows χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), οι υπηρεσίες Terminal Services που παλαιότερα ονομάζονταν:10</span><span class="sxs-lookup"><span data-stu-id="b482a-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b482a-104">Πρέπει να έχετε μια συνδρομή Microsoft 365 που περιλαμβάνει εφαρμογές της Microsoft 365 για μεγάλες επιχειρήσεις, όπως το Office 365 για μεγάλες επιχειρήσεις E3 ή για μεγάλες επιχειρήσεις E5.</span><span class="sxs-lookup"><span data-stu-id="b482a-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="b482a-105">Οι εφαρμογές microsoft 365 για επιχειρήσεις και οι εφαρμογές Microsoft 365 για προγράμματα Premium για επιχειρήσεις δεν περιλαμβάνουν εφαρμογές της Microsoft 365 για επιχειρήσεις.</span><span class="sxs-lookup"><span data-stu-id="b482a-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="b482a-106">Πρέπει να ενεργοποιήσετε την [ενεργοποίηση κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b482a-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="b482a-107">Εάν θέλετε να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, ***το οποίο χρησιμοποιεί προεπιλεγμένες ρυθμίσεις εγκατάστασης***, χρησιμοποιήστε τα ακόλουθα βήματα.</span><span class="sxs-lookup"><span data-stu-id="b482a-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="b482a-108">Μπορείτε επίσης να κάνετε λήψη και εκτέλεση του [Βοηθού υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για επιχειρήσεις σε κατάσταση ενεργοποίησης κοινόχρηστου υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="b482a-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="b482a-109">Ελέγξτε τι συνδρομή microsoft 365 που έχετε.</span><span class="sxs-lookup"><span data-stu-id="b482a-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="b482a-110">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="b482a-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="b482a-111">Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική συνδρομή Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b482a-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="b482a-112">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="b482a-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="b482a-113">Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές του Microsoft 365, καταργήστε την εγκατάστασή του.</span><span class="sxs-lookup"><span data-stu-id="b482a-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="b482a-114">Για παράδειγμα, μεταβαίνωσε στον Πίνακα \> Ελέγχου Κατάργηση εγκατάστασης ενός προγράμματος.</span><span class="sxs-lookup"><span data-stu-id="b482a-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="b482a-115">Καταργήστε την εγκατάσταση [χρησιμοποιώντας το Βοηθό υποστήριξης και αποκατάστασης της Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν εξαντλείστε προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="b482a-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="b482a-116">Στο διακομιστή RDS, συνδεθείτε στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή και [εγκαταστήστε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b482a-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="b482a-117">Μετά την εγκατάσταση του Office, ***μην ανοίξετε ή εισέλθετε σε*** εφαρμογές του Office.</span><span class="sxs-lookup"><span data-stu-id="b482a-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="b482a-118">Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση κοινόχρηστου υπολογιστή με επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="b482a-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="b482a-119">Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε Εκτέλεση.</span><span class="sxs-lookup"><span data-stu-id="b482a-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="b482a-120">Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.</span><span class="sxs-lookup"><span data-stu-id="b482a-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="b482a-121">Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε στον Επεξεργαστή Μητρώου (Registry Editor) να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="b482a-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="b482a-122">Στον Επεξεργαστή Μητρώου (Registry Editor), προσθέστε μια τιμή συμβολοσειράς της **άδειας χρήσης κοινόχρηστου υπολογιστή** με ρύθμιση 1 υπό HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="b482a-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="b482a-123">Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [βεβαιωθείτε ότι είναι ενεργοποιημένη η ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b482a-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="b482a-124">Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το Εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b482a-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="b482a-125">Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b482a-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  