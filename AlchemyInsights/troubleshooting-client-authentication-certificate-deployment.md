---
title: Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555000"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="72750-102">Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη</span><span class="sxs-lookup"><span data-stu-id="72750-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="72750-103">Τα προφίλ πιστοποιητικών Intune NDES/SCEP και PKCS/PFX Client χρησιμοποιούνται συνήθως σε συνδυασμό με άλλους τύπους προφίλ, όπως Wifi, VPN και ηλεκτρονικό ταχυδρομείο, ώστε να επιτρέπεται στους χρήστες ο έλεγχος ταυτότητας σε εταιρικούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="72750-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="72750-104">Όταν αυτοί οι τύποι προφίλ συνδέονται με ένα προφίλ πιστοποιητικού προγράμματος-πελάτη εξαρτώνται από την επιτυχή ανάπτυξη αυτού του προφίλ.</span><span class="sxs-lookup"><span data-stu-id="72750-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="72750-105">Η αρχική εγκατάσταση υποδομής και η συσχετισμένη ρύθμιση παραμέτρων του προφίλ πιστοποιητικού προγράμματος-πελάτη συχνά απαιτούν αντιμετώπιση προβλημάτων.</span><span class="sxs-lookup"><span data-stu-id="72750-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="72750-106">Για έναν οδηγό βήμα προς βήμα για την επιτυχή εγκατάσταση της σύνδεσης NDES και οδηγίες αντιμετώπισης προβλημάτων για την απομόνωση ζητημάτων με την ανάπτυξη πιστοποιητικού, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="72750-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="72750-107">Ρύθμιση παραμέτρων υποδομής για υποστήριξη SCEP με Intune</span><span class="sxs-lookup"><span data-stu-id="72750-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="72750-108">Επισκόπηση για την αντιμετώπιση προβλημάτων προφίλ πιστοποιητικών SCEP με το Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="72750-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="72750-109">Χρησιμοποιήστε τις αναφερόμενες δέσμες ενεργειών powershell για να επαληθεύσετε τις παραμέτρους σας.</span><span class="sxs-lookup"><span data-stu-id="72750-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="72750-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δέσμες ενεργειών επαλήθευσης σύνδεσης πιστοποιητικού Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="72750-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="72750-111">**Άλλα κοινά ζητήματα**</span><span class="sxs-lookup"><span data-stu-id="72750-111">**Other common issues**</span></span>

<span data-ttu-id="72750-112">**Όταν προσπαθώ να εγκαταστήσω τη σύνδεση πιστοποιητικού Intune στο διακομιστή σύνδεσης NDES, λαμβάνω το μήνυμα, "Δεν είναι δυνατή η επαλήθευση του κωδικού πρόσβασης στην αίτηση πιστοποιητικού. Μπορεί να έχει ήδη χρησιμοποιηθεί. Αποκτήστε έναν νέο κωδικό πρόσβασης για να υποβάλετε με αυτήν την αίτηση."**</span><span class="sxs-lookup"><span data-stu-id="72750-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="72750-113">Αυτό το μήνυμα σημαίνει ότι πρέπει να εκτελέσετε την εγκατάσταση σύνδεσης πιστοποιητικού ως διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="72750-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="72750-114">Σε ορισμένα περιβάλλοντα, οι διακομιστές όπου εκτελείται το πιστοποιητικό Intune πρέπει να χρησιμοποιούν ένα διακομιστή μεσολάβησης για να συνδεθούν με το Intune και έτσι η σύνδεση πιστοποιητικού πρέπει να χρησιμοποιεί διακομιστή μεσολάβησης.</span><span class="sxs-lookup"><span data-stu-id="72750-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="72750-115">Σε ορισμένες περιπτώσεις, η σύνδεση NDES αγνοεί τις ρυθμισμένες ρυθμίσεις διακομιστή μεσολάβησης και ίσως χρειαστεί να ρυθμίσετε τις παραμέτρους του διακομιστή μεσολάβησης κατά την εκτέλεση στο περιβάλλον ασφαλείας του LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="72750-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="72750-116">Η λύση είναι να εκτελέσετε τον Internet Explorer ως SYSTEM και να ρυθμίσετε τις παραμέτρους ενός διακομιστή μεσολάβησης στον IE.</span><span class="sxs-lookup"><span data-stu-id="72750-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="72750-117">Μετά από μια επανεκκίνηση της υπηρεσίας σύνδεσης Intune, η σύνδεση NDES συνδέεται με το Intune.</span><span class="sxs-lookup"><span data-stu-id="72750-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="72750-118">**Οι συσκευές χρήστη δεν λαμβάνουν πλέον πιστοποιητικά SCEP από το NDES.**</span><span class="sxs-lookup"><span data-stu-id="72750-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="72750-119">Είναι πιθανό το πιστοποιητικό ελέγχου ταυτότητας υπολογιστή-πελάτη που εκδόθηκε στο διακομιστή NDES και καθορίστηκε κατά την εγκατάσταση σύνδεσης NDES, να έχει λήξει ή να λείπει.</span><span class="sxs-lookup"><span data-stu-id="72750-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="72750-120">Για να επιλύσετε:</span><span class="sxs-lookup"><span data-stu-id="72750-120">To resolve:</span></span> 
 
1. <span data-ttu-id="72750-121">Καταργήστε την εγκατάσταση της σύνδεσης NDES.</span><span class="sxs-lookup"><span data-stu-id="72750-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="72750-122">Χρησιμοποιήστε αυτές τις λεπτομέρειες για να ζητήσετε ένα νέο πιστοποιητικό ελέγχου ταυτότητας υπολογιστή-πελάτη ή διακομιστή:</span><span class="sxs-lookup"><span data-stu-id="72750-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="72750-123">Όνομα θέματος: CN=εξωτερικό fqdn</span><span class="sxs-lookup"><span data-stu-id="72750-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="72750-124">Εναλλακτικό όνομα θέματος (και τα δύο απαιτούνται): DNS=εξωτερικό fqdn, DNS=εσωτερικό fqdn</span><span class="sxs-lookup"><span data-stu-id="72750-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="72750-125">Εγκαταστήστε ξανά τη σύνδεση NDES με το νέο πιστοποιητικό.</span><span class="sxs-lookup"><span data-stu-id="72750-125">Reinstall the NDES connector with the new certificate.</span></span>