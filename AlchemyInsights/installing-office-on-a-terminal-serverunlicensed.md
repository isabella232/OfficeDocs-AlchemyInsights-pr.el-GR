---
title: Εγκατάσταση του Office σε διακομιστή τερματικού-χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735389"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="c8f1d-102">Εγκατάσταση του Office σε διακομιστή τερματικού</span><span class="sxs-lookup"><span data-stu-id="c8f1d-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="c8f1d-103">Για την ανάπτυξη του Office 365 ProPlus σε ένα διακομιστή των Windows χρησιμοποιώντας υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), παλαιότερα ονομαζόταν υπηρεσίες Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="c8f1d-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="c8f1d-104">Πρέπει να έχετε ένα σχέδιο 365 του Office που περιλαμβάνει το Office 365 ProPlus, όπως το Office 365 Enterprise ε ή Enterprise Ε+.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="c8f1d-105">Τα σχέδια Office 365 Business και Office 365 Business Premium δεν περιλαμβάνουν το Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="c8f1d-106">Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="c8f1d-107">Εάν θέλετε να εγκαταστήσετε το Office 365 ProPlus σε RDS από το κέντρο διαχείρισης της Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="c8f1d-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="c8f1d-108">Ελέγξτε το σχέδιο 365 του Office που έχετε.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="c8f1d-109">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="c8f1d-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="c8f1d-110">Εάν είναι απαραίτητο, μεταβείτε σε διαφορετικό σχέδιο του Office 365.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="c8f1d-111">Μάθετε πώς</span><span class="sxs-lookup"><span data-stu-id="c8f1d-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="c8f1d-112">Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιαδήποτε άλλα σχέδια του Office 365, απεγκαταστήστε το.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="c8f1d-113">Για παράδειγμα, πηγαίνοντας στον πίνακα \> ελέγχου απεγκατάσταση ενός προγράμματος.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="c8f1d-114">Κατάργηση εγκατάστασης χρησιμοποιώντας [την υποστήριξη της Microsoft και τον βοηθό αποκατάστασης](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν εκτελείτε ζητήματα.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="c8f1d-115">Στο διακομιστή RDS, εισέλθετε στο κέντρο διαχείρισης Microsoft 365 με το λογαριασμό διαχειριστή σας και εγκαταστήστε το [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="c8f1d-116">Μετά την εγκατάσταση του Office, ***Μην ανοίξετε ή εισέλθετε*** σε οποιεσδήποτε εφαρμογές του Office.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="c8f1d-117">Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή με την επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="c8f1d-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="c8f1d-118">Κάντε δεξιό κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="c8f1d-119">Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="c8f1d-120">Επιλέξτε Yes όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="c8f1d-121">Στο πρόγραμμα επεξεργασίας μητρώου, προσθέστε μια τιμή συμβολοσειράς της κοινής **χρήσης υπολογιστή** με ρύθμιση 1 κάτω από το HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office</span><span class="sxs-lookup"><span data-stu-id="c8f1d-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="c8f1d-122">Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [Επιβεβαιώστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="c8f1d-123">Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, οδηγίες εγκατάστασης και οδηγίες σχετικά με προσαρμοσμένες εγκαταστάσεις, χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στην ενότητα [ανάπτυξη Office 365 ProPlus, χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="c8f1d-124">Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση του κοινόχρηστου υπολογιστή, ανατρέξτε στο [θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  