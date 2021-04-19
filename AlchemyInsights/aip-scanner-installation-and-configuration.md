---
title: 'Σαρωτής AIP: εγκατάσταση και ρύθμιση παραμέτρων'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821663"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7bccf-102">Σαρωτής AIP: εγκατάσταση και ρύθμιση παραμέτρων</span><span class="sxs-lookup"><span data-stu-id="7bccf-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7bccf-103">**Για να εγκαταστήσετε το σαρωτή AIP, ακολουθήστε τις προτεινόμενες οδηγίες:**</span><span class="sxs-lookup"><span data-stu-id="7bccf-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7bccf-104">Εάν κάνετε αναβάθμιση και δεν εκτελείτε καθαρή εγκατάσταση, βεβαιωθείτε ότι έχετε ακολουθήσει τις οδηγίες για την αναβάθμιση του [σαρωτή προστασίας](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) πληροφοριών Azure και για το ενοποιημένο πρόγραμμα-πελάτη σήμανσης, ανατρέξτε στο θέμα αναβάθμιση του σαρωτή Προστασίας [πληροφοριών Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="7bccf-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7bccf-105">Βεβαιωθείτε ότι συμμορφώνεστε με όλα τα [Τείχη προστασίας και τις απαιτήσεις ρυθμίσεων υποδομής δικτύου.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="7bccf-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7bccf-106">Βεβαιωθείτε ότι οι [πολιτικές σας έχουν](https://docs.microsoft.com/azure/information-protection/configure-policy) οριστεί σε αυτόματη σήμανση ή ότι έχουν μια προεπιλεγμένη ετικέτα στην πολιτική.</span><span class="sxs-lookup"><span data-stu-id="7bccf-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7bccf-107">Βεβαιωθείτε ότι ο σχετικός τύπος αρχείου έχει ρυθμιστεί για ετικέτα/προστασία, όπως περιγράφεται στους τύπους [αρχείων που υποστηρίζονται από το πρόγραμμα-πελάτη Προστασίας πληροφοριών Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="7bccf-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7bccf-108">Επιπλέον, εάν θέλετε να αλλάξετε την προεπιλεγμένη συμπεριφορά, ακολουθήστε τις παρακάτω οδηγίες: [Αλλαγή του προεπιλεγμένου επιπέδου προστασίας αρχείων.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="7bccf-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7bccf-109">Βεβαιωθείτε ότι ο λογαριασμός χρήστη που έχει ρυθμιστεί για την εκτέλεση της υπηρεσίας σαρωτή έχει δικαιώματα πρόσβασης σε όλα τα ρυθμισμένα αποθετήρια.</span><span class="sxs-lookup"><span data-stu-id="7bccf-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7bccf-110">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα, εξαγάγετε τα αρχεία καταγραφής του σαρωτή και προσθέστε τα στο δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="7bccf-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7bccf-111">**Εξαγωγή αρχείων καταγραφής του Σαρωτή προστασίας πληροφοριών Azure**</span><span class="sxs-lookup"><span data-stu-id="7bccf-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7bccf-112">Μεταβείτε στο %localappdata%\Microsoft\MSIP κάτω από το περιβάλλον χρήστη που εκτελεί την υπηρεσία σαρωτή.</span><span class="sxs-lookup"><span data-stu-id="7bccf-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7bccf-113">Συμπίεση όλων των περιεχομένων κάτω από το φάκελο MSIP.</span><span class="sxs-lookup"><span data-stu-id="7bccf-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7bccf-114">Αποθηκεύστε τα αρχεία καταγραφής στην επιλογή θέσης σας και επισυνάψτε τα στην αίτηση εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="7bccf-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7bccf-115">Μπορείτε επίσης να χρησιμοποιήσετε [το Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="7bccf-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7bccf-116">**Για πρόσθετες πληροφορίες, ανατρέξτε στο θέμα:**</span><span class="sxs-lookup"><span data-stu-id="7bccf-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7bccf-117">Ανάπτυξη του σαρωτή προστασίας πληροφοριών Azure για την αυτόματη ταξινόμηση και προστασία αρχείων</span><span class="sxs-lookup"><span data-stu-id="7bccf-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7bccf-118">Καθορισμός και χρήση της παραμέτρου Διακριτικού για το Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="7bccf-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7bccf-119">Εκτέλεση κύκλου εντοπισμού και προβολή αναφορών για το σαρωτή</span><span class="sxs-lookup"><span data-stu-id="7bccf-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7bccf-120">Αναθεώρηση τεκμηρίωσης της Προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="7bccf-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7bccf-121">Απαιτήσεις για την Προστασία πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="7bccf-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7bccf-122">Λήψη προγράμματος-πελάτη Προστασίας πληροφοριών Azure</span><span class="sxs-lookup"><span data-stu-id="7bccf-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
