---
title: Ενεργοποίηση ελέγχου ταυτότητας ΚΑΙ αντιμετώπισης προβλημάτων SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077651"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="74763-102">Ενεργοποίηση ελέγχου ταυτότητας ΚΑΙ αντιμετώπισης προβλημάτων SMTP</span><span class="sxs-lookup"><span data-stu-id="74763-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="74763-103">Εάν θέλετε να ενεργοποιήσετε τον έλεγχο ταυτότητας SMTP για ένα γραμματοκιβώτιο ή εάν εμφανίζεται ένα σφάλμα "Ο υπολογιστής-πελάτης δεν έχει ελεγχθεί", "Ο έλεγχος ταυτότητας απέτυχε" ή το σφάλμα "SmtpClientAuthentication" με κωδικό 5.7.57 ή 5.7.3 ή 5.7.139 όταν προσπαθείτε να κάνετε αναμετάδοση ηλεκτρονικού ταχυδρομείου με έλεγχο ταυτότητας μιας συσκευής ή εφαρμογής με το Microsoft 365, εκτελέστε αυτές τις τρεις ενέργειες για να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="74763-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="74763-104">Απενεργοποιήστε [τις προεπιλογές ασφαλείας του Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ενεργοποιώντας **την επιλογή "Ενεργοποίηση προεπιλογών ασφαλείας"** σε **"Όχι".**</span><span class="sxs-lookup"><span data-stu-id="74763-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="74763-105">a.</span><span class="sxs-lookup"><span data-stu-id="74763-105">a.</span></span> <span data-ttu-id="74763-106">Πραγματοποιήστε είσοδο στην πύλη Azure ως διαχειριστής ασφαλείας, διαχειριστής πρόσβασης υπό όρους ή καθολικός διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="74763-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="74763-107">b.</span><span class="sxs-lookup"><span data-stu-id="74763-107">b.</span></span> <span data-ttu-id="74763-108">Μεταβείτε στην επιλογή Azure Active Directory > **Ιδιότητες.**</span><span class="sxs-lookup"><span data-stu-id="74763-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="74763-109">c.</span><span class="sxs-lookup"><span data-stu-id="74763-109">c.</span></span> <span data-ttu-id="74763-110">Επιλέξτε **"Διαχείριση προεπιλογών ασφαλείας".**</span><span class="sxs-lookup"><span data-stu-id="74763-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="74763-111">d.</span><span class="sxs-lookup"><span data-stu-id="74763-111">d.</span></span> <span data-ttu-id="74763-112">Ορισμός **προεπιλογών ενεργοποίησης ασφαλείας** σε **"Όχι".**</span><span class="sxs-lookup"><span data-stu-id="74763-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="74763-113">e.</span><span class="sxs-lookup"><span data-stu-id="74763-113">e.</span></span> <span data-ttu-id="74763-114">Επιλέξτε **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="74763-114">Select **Save**.</span></span>

2. <span data-ttu-id="74763-115">[Ενεργοποίηση υποβολής SMTP προγράμματος-πελάτη](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) στο γραμματοκιβώτιο με άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="74763-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="74763-116">a.</span><span class="sxs-lookup"><span data-stu-id="74763-116">a.</span></span> <span data-ttu-id="74763-117">Από το Κέντρο διαχείρισης Microsoft 365, μεταβείτε στην επιλογή **"Ενεργοί χρήστες"** και επιλέξτε το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="74763-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="74763-118">b.</span><span class="sxs-lookup"><span data-stu-id="74763-118">b.</span></span> <span data-ttu-id="74763-119">Μεταβείτε στην καρτέλα "Αλληλογραφία" και, στην περιοχή **"Εφαρμογές ηλεκτρονικού ταχυδρομείου",** επιλέξτε **"Διαχείριση εφαρμογών ηλεκτρονικού ταχυδρομείου".**</span><span class="sxs-lookup"><span data-stu-id="74763-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="74763-120">d.</span><span class="sxs-lookup"><span data-stu-id="74763-120">d.</span></span> <span data-ttu-id="74763-121">Βεβαιωθείτε ότι είναι **επιλεγμένο το SMTP** με έλεγχο ταυτότητας (ενεργοποιημένο).</span><span class="sxs-lookup"><span data-stu-id="74763-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="74763-122">e.</span><span class="sxs-lookup"><span data-stu-id="74763-122">e.</span></span> <span data-ttu-id="74763-123">Επιλέξτε **"Αποθήκευση αλλαγών".**</span><span class="sxs-lookup"><span data-stu-id="74763-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="74763-124">[Απενεργοποιήστε τον έλεγχο ταυτότητας πολλών παραγόντων (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) στο γραμματοκιβώτιο με άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="74763-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="74763-125">a.</span><span class="sxs-lookup"><span data-stu-id="74763-125">a.</span></span> <span data-ttu-id="74763-126">Μεταβείτε στην Κέντρο διαχείρισης Microsoft 365 και, στο αριστερό μενού περιήγησης, επιλέξτε **"Χρήστες**  >  **ενεργοί χρήστες".**</span><span class="sxs-lookup"><span data-stu-id="74763-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="74763-127">b.</span><span class="sxs-lookup"><span data-stu-id="74763-127">b.</span></span> <span data-ttu-id="74763-128">Επιλέξτε έλεγχο **ταυτότητας πολλών παραγόντων.**</span><span class="sxs-lookup"><span data-stu-id="74763-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="74763-129">c.</span><span class="sxs-lookup"><span data-stu-id="74763-129">c.</span></span> <span data-ttu-id="74763-130">Επιλέξτε το χρήστη και απενεργοποιήστε **την ταυτότητα πολλών παραγόντων.**</span><span class="sxs-lookup"><span data-stu-id="74763-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
