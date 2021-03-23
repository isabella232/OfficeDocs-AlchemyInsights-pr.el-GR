---
title: Ρύθμιση παραμέτρων σημείου σύνδεσης υπηρεσίας (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036141"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="76f04-102">Ρύθμιση παραμέτρων σημείου σύνδεσης υπηρεσίας (SCP)</span><span class="sxs-lookup"><span data-stu-id="76f04-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="76f04-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="76f04-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="76f04-104">**Αιτία:** Δεν είναι δυνατή η ανάγνωση του αντικειμένου SCP και η λήψη των πληροφοριών μισθωτή Azure AD</span><span class="sxs-lookup"><span data-stu-id="76f04-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="76f04-105">**Επίλυση:** Ανατρέξτε στην ενότητα "Ρύθμιση [παραμέτρων σημείου σύνδεσης υπηρεσίας"](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="76f04-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="76f04-106">**Σχέδιο δράσης**</span><span class="sxs-lookup"><span data-stu-id="76f04-106">**Action plan**</span></span>

- <span data-ttu-id="76f04-107">Ελέγξτε εάν η συσκευή έχει λάβει το GPO για την ελεγχόμενη επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="76f04-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="76f04-108">Βεβαιωθείτε ότι το GPO έχει δημιουργήσει τα κλειδιά μητρώου.</span><span class="sxs-lookup"><span data-stu-id="76f04-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="76f04-109">Βεβαιωθείτε ότι έχετε δημιουργήσει 2 κλειδιά με το αναγνωριστικό καταλόγου και τον τομέα onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="76f04-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="76f04-110">**Ρύθμιση παραμέτρων μητρώου από την πλευρά του προγράμματος-πελάτη για SCP**</span><span class="sxs-lookup"><span data-stu-id="76f04-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="76f04-111">Χρησιμοποιήστε το παρακάτω παράδειγμα για να δημιουργήσετε ένα αντικείμενο πολιτικής ομάδας (GPO) για να αναπτύξετε μια ρύθμιση μητρώου που ρυθμίζει τις παραμέτρους μιας καταχώρησης SCP στο μητρώο των συσκευών σας.</span><span class="sxs-lookup"><span data-stu-id="76f04-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="76f04-112">Ανοίξτε μια κονσόλα διαχείρισης πολιτικής ομάδας και δημιουργήστε ένα νέο GPO στον τομέα σας.</span><span class="sxs-lookup"><span data-stu-id="76f04-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="76f04-113">Δώστε ένα όνομα στο GPO που μόλις δημιουργήσατε (για παράδειγμα, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="76f04-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="76f04-114">Επεξεργαστείτε το GPO και εντοπίστε την ακόλουθη διαδρομή: Ρυθμίσεις **παραμέτρων υπολογιστή > προτιμήσεις > ρυθμίσεις των Windows > Μητρώο.**</span><span class="sxs-lookup"><span data-stu-id="76f04-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="76f04-115">Κάντε δεξί κλικ στο **Μητρώο και** επιλέξτε **"Νέο > μητρώου".**</span><span class="sxs-lookup"><span data-stu-id="76f04-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="76f04-116">Στην καρτέλα **"Γενικά",** ρυθμίστε τις παραμέτρους για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="76f04-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="76f04-117">**Ενέργεια:** Ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="76f04-117">**Action**: Update</span></span>
    
- <span data-ttu-id="76f04-118">**Ομάδα**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="76f04-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="76f04-119">**Διαδρομή κλειδιού:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="76f04-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="76f04-120">**Όνομα τιμής:** TenantId</span><span class="sxs-lookup"><span data-stu-id="76f04-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="76f04-121">**Τύπος τιμής:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="76f04-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="76f04-122">**Δεδομένα τιμής:** Το αναγνωριστικό GUID ή καταλόγου της παρουσίας azure AD (Αυτή η τιμή μπορεί να βρεθεί στην πύλη **Azure > Azure Active Directory > Ιδιότητες > αναγνωριστικό καταλόγου)**</span><span class="sxs-lookup"><span data-stu-id="76f04-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="76f04-123">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="76f04-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="76f04-124">Κάντε δεξί κλικ στο **Μητρώο και** επιλέξτε **"Νέο > μητρώου".**</span><span class="sxs-lookup"><span data-stu-id="76f04-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="76f04-125">Στην καρτέλα **"Γενικά",** ρυθμίστε τις παραμέτρους για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="76f04-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="76f04-126">**Ενέργεια:** Ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="76f04-126">**Action**: Update</span></span>
    
- <span data-ttu-id="76f04-127">**Ομάδα**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="76f04-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="76f04-128">**Διαδρομή κλειδιού:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="76f04-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="76f04-129">**Όνομα τιμής:** Όνομα μισθωτή</span><span class="sxs-lookup"><span data-stu-id="76f04-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="76f04-130">**Τύπος τιμής:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="76f04-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="76f04-131">**Δεδομένα τιμών:** Το επαληθευμένο όνομα τομέα σας, εάν χρησιμοποιείτε ομόσπονδο περιβάλλον, όπως AD FS.</span><span class="sxs-lookup"><span data-stu-id="76f04-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="76f04-132">Το επαληθευμένο όνομα τομέα ή το onmicrosoft.com τομέα σας (για παράδειγμα, contoso.onmicrosoft).com εάν χρησιμοποιείτε διαχειριζόμενο περιβάλλον</span><span class="sxs-lookup"><span data-stu-id="76f04-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="76f04-133">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="76f04-133">Click **OK**.</span></span>

7. <span data-ttu-id="76f04-134">Κλείστε το πρόγραμμα επεξεργασίας για το GPO που μόλις δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="76f04-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="76f04-135">Συνδέστε το νέο GPO με την επιθυμητή OU που περιέχει υπολογιστές που συνδέονται με τομέα και ανήκουν στον ελεγχόμενο πληθυσμό της συνάθροισης.</span><span class="sxs-lookup"><span data-stu-id="76f04-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="76f04-136">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ελεγχόμενη επικύρωση υβριδικού συνδέσμου Azure AD - Azure AD | Συσκευές που είναι συνδεδεμένες](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) στο Azure Active Directory και  [αντιμετώπιση προβλημάτων με υβριδικές συσκευές | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="76f04-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









