---
title: Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658986"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="486c3-102">Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη</span><span class="sxs-lookup"><span data-stu-id="486c3-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="486c3-103">Τα προφίλ των πιστοποιητικών προγράμματος-πελάτη Intune NDES/SCEP και PKCS/PFX χρησιμοποιούνται συνήθως σε συνδυασμό με άλλους τύπους προφίλ, όπως το WiFi, το VPN και το ηλεκτρονικό ταχυδρομείο, για να επιτρέπουν στους χρήστες να πραγματοποιούν έλεγχο ταυτότητας σε εταιρικούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="486c3-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="486c3-104">Όταν αυτοί οι τύποι προφίλ είναι συνδεδεμένοι με ένα προφίλ πιστοποιητικού προγράμματος-πελάτη εξαρτώνται από την επιτυχή ανάπτυξη αυτού του προφίλ.</span><span class="sxs-lookup"><span data-stu-id="486c3-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="486c3-105">Η αρχική ρύθμιση υποδομής και η συσχετισμένη ρύθμιση παραμέτρων του προφίλ πιστοποιητικού προγράμματος-πελάτη απαιτούν συχνά αντιμετώπιση προβλημάτων.</span><span class="sxs-lookup"><span data-stu-id="486c3-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="486c3-106">Για έναν οδηγό βήμα προς βήμα για την επιτυχή ρύθμιση της σύνδεσης NDES και τις οδηγίες αντιμετώπισης προβλημάτων για την απομόνωση ζητημάτων με την ανάπτυξη πιστοποιητικών, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="486c3-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="486c3-107">Ρύθμιση παραμέτρων υποδομής για την υποστήριξη του SCEP με το Intune</span><span class="sxs-lookup"><span data-stu-id="486c3-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="486c3-108">Επισκόπηση για την αντιμετώπιση προβλημάτων με τα προφίλ πιστοποιητικών SCEP με το Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="486c3-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="486c3-109">Χρησιμοποιήστε τις συσχετισμένες δέσμες ενεργειών του PowerShell για να επαληθεύσετε τις ρυθμίσεις παραμέτρων σας.</span><span class="sxs-lookup"><span data-stu-id="486c3-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="486c3-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [δέσμες ενεργειών επαλήθευσης της σύνδεσης πιστοποιητικού Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="486c3-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="486c3-111">**Άλλα συνηθισμένα προβλήματα**</span><span class="sxs-lookup"><span data-stu-id="486c3-111">**Other common issues**</span></span>

<span data-ttu-id="486c3-112">**Όταν προσπαθώ να εγκαταστήσω τη σύνδεση πιστοποιητικού Intune στο διακομιστή σύνδεσης NDES, παίρνω το μήνυμα "δεν είναι δυνατή η επαλήθευση του κωδικού πρόσβασης στην αίτηση πιστοποιητικού. Μπορεί να έχει ήδη χρησιμοποιηθεί. Αποκτήστε έναν νέο κωδικό πρόσβασης για να υποβάλετε με αυτή την αίτηση. "**</span><span class="sxs-lookup"><span data-stu-id="486c3-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="486c3-113">Αυτό το μήνυμα σημαίνει ότι πρέπει να εκτελέσετε την εγκατάσταση της σύνδεσης πιστοποιητικού ως διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="486c3-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="486c3-114">Σε ορισμένα περιβάλλοντα, οι διακομιστές όπου εκτελείται το πιστοποιητικό Intune πρέπει να χρησιμοποιούν ένα διακομιστή μεσολάβησης για να συνδεθούν με το Intune και, επομένως, η γραμμή σύνδεσης του πιστοποιητικού πρέπει να χρησιμοποιεί ένα διακομιστή μεσολάβησης.</span><span class="sxs-lookup"><span data-stu-id="486c3-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="486c3-115">Σε ορισμένες περιπτώσεις, η γραμμή σύνδεσης του NDES παραβλέπει τις ρυθμισμένες ρυθμίσεις του διακομιστή μεσολάβησης και μπορεί να είναι απαραίτητο να ρυθμίσετε τις παραμέτρους του διακομιστή μεσολάβησης κατά την εκτέλεση στο περιβάλλον ασφαλείας του τοπικού συστήματος.</span><span class="sxs-lookup"><span data-stu-id="486c3-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="486c3-116">Η λύση είναι να εκτελέσετε τον Internet Explorer ως σύστημα και να ρυθμίσετε τις παραμέτρους ενός διακομιστή μεσολάβησης στον IE.</span><span class="sxs-lookup"><span data-stu-id="486c3-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="486c3-117">Μετά την επανεκκίνηση της υπηρεσίας σύνδεσης Intune, η σύνδεση NDES συνδέεται με το Intune.</span><span class="sxs-lookup"><span data-stu-id="486c3-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="486c3-118">**Οι συσκευές χρήστη δεν λαμβάνουν πλέον πιστοποιητικά SCEP από το NDES.**</span><span class="sxs-lookup"><span data-stu-id="486c3-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="486c3-119">Είναι πιθανό ότι το πιστοποιητικό ελέγχου ταυτότητας υπολογιστή-πελάτη που έχει εκδοθεί στο διακομιστή NDES και έχει καθοριστεί κατά τη διάρκεια της εγκατάστασης του NDES Connector έχει λήξει ή λείπει.</span><span class="sxs-lookup"><span data-stu-id="486c3-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="486c3-120">Για να επιλύσετε:</span><span class="sxs-lookup"><span data-stu-id="486c3-120">To resolve:</span></span> 
 
1. <span data-ttu-id="486c3-121">Καταργήστε την εγκατάσταση της σύνδεσης NDES.</span><span class="sxs-lookup"><span data-stu-id="486c3-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="486c3-122">Χρησιμοποιήστε αυτές τις λεπτομέρειες για να ζητήσετε έναν νέο έλεγχο ταυτότητας υπολογιστή-πελάτη ή ένα πιστοποιητικό ελέγχου ταυτότητας διακομιστή:</span><span class="sxs-lookup"><span data-stu-id="486c3-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="486c3-123">Όνομα θέματος: CN = εξωτερικό FQDN</span><span class="sxs-lookup"><span data-stu-id="486c3-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="486c3-124">Εναλλακτικό όνομα θέματος (απαιτούνται και τα δύο): DNS = εξωτερικό FQDN, DNS = εσωτερικό FQDN</span><span class="sxs-lookup"><span data-stu-id="486c3-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="486c3-125">Επανεγκατάσταση της σύνδεσης NDES με το νέο πιστοποιητικό.</span><span class="sxs-lookup"><span data-stu-id="486c3-125">Reinstall the NDES connector with the new certificate.</span></span>