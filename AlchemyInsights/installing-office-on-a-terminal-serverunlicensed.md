---
title: Την εγκατάσταση του office σε ένα διακομιστή τερματικού - χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918974"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="6edbb-102">Την εγκατάσταση του Office σε ένα διακομιστή τερματικού</span><span class="sxs-lookup"><span data-stu-id="6edbb-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="6edbb-103">Για την ανάπτυξη του Office 365 ProPlus σε ένα διακομιστή των Windows χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), παλιότερα με το όνομα των υπηρεσιών Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="6edbb-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="6edbb-p101">Πρέπει να έχετε ένα πρόγραμμα Office 365 που περιλαμβάνει το Office 365 ProPlus, όπως E3 Enterprise του Office 365 ή εταιρικού E5. Τα σχέδια Office 365 επιχειρήσεων και πριμοδότηση επαγγελματική του Office 365 δεν περιλαμβάνουν Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="6edbb-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="6edbb-106">Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση κοινόχρηστο υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6edbb-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="6edbb-107">Εάν θέλετε να εγκαταστήσετε το Office 365 ProPlus σε RDS από την πύλη Office 365, \*\* *που χρησιμοποιούν τις προεπιλεγμένες ρυθμίσεις εγκατάστασης* \*\*, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="6edbb-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="6edbb-p102">Ελέγξτε τι σχέδιο Office 365 που έχετε. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="6edbb-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="6edbb-p103">Εάν είναι απαραίτητο, μεταβείτε σε ένα διαφορετικό Office 365 σχεδιασμό. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="6edbb-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="6edbb-p104">Αν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS, χρησιμοποιώντας οποιαδήποτε άλλα σχέδια Office 365, καταργήσετε την εγκατάστασή του. Για παράδειγμα, μεταβαίνοντας τον πίνακα ελέγχου \> κατάργηση εγκατάστασης ενός προγράμματος. Καταργήστε την εγκατάσταση χρησιμοποιώντας την [υπηρεσία υποστήριξης της Microsoft και αποκατάστασης του Βοηθού](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν εκτελείτε σε θέματα.</span><span class="sxs-lookup"><span data-stu-id="6edbb-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="6edbb-115">Στο διακομιστή RDS, εισέλθετε στην πύλη Office 365 με το λογαριασμό διαχειριστή και να [εγκαταστήσετε το Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="6edbb-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="6edbb-116">Μετά την εγκατάσταση του Office, \*\* *δεν ανοίξετε ή να εισέλθετε* \*\* για τις εφαρμογές του Office.</span><span class="sxs-lookup"><span data-stu-id="6edbb-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="6edbb-117">Στο διακομιστή RDS, δυνατή Ενεργοποίηση κοινόχρηστο υπολογιστή με επεξεργασία του μητρώου ακολουθώντας τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="6edbb-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="6edbb-p105">Κάντε δεξιό κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.</span><span class="sxs-lookup"><span data-stu-id="6edbb-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="6edbb-120">Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε τον Επεξεργαστή μητρώου για να κάνετε αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="6edbb-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="6edbb-121">Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς **SharedComputerLicensing** με ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="6edbb-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="6edbb-122">Στο διακομιστή RDS, \*\* *εισέλθετε ως ένας τελικός χρήστης* \*\* και [Βεβαιωθείτε ότι είναι ενεργοποιημένη η ενεργοποίηση κοινόχρηστο υπολογιστή για Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="6edbb-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="6edbb-123">Για περισσότερες λεπτομέρειες σχετικά με προϋποθέσεις, οδηγίες και κατευθύνσεις σχετικά με προσαρμοσμένες εγκαταστάσεις, χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε [Αναπτύσσουν Office 365 ProPlus, χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="6edbb-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="6edbb-124">Για να διορθώσετε τα σφάλματα που αφορούν την ενεργοποίηση κοινόχρηστο υπολογιστή, ανατρέξτε στην [Αντιμετώπιση προβλημάτων με ενεργοποίηση κοινόχρηστο υπολογιστή για Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6edbb-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

