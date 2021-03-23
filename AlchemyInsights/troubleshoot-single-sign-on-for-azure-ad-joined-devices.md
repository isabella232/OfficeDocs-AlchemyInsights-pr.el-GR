---
title: Αντιμετώπιση προβλημάτων μονής σύνδεσης για συσκευές που είναι συνδεδεμένες στο Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036169"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="5d162-102">Αντιμετώπιση προβλημάτων μονής σύνδεσης για συσκευές που είναι συνδεδεμένες στο Azure AD</span><span class="sxs-lookup"><span data-stu-id="5d162-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="5d162-103">Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5d162-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="5d162-104">[Τρόπος: Ο σχεδιασμός της υβριδικής](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) εφαρμογής συμμετοχής στο Azure Active Directory σάς παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.</span><span class="sxs-lookup"><span data-stu-id="5d162-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="5d162-105">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες στο [Azure AD για Single-Sign εσωτερικής εγκατάστασης χρησιμοποιώντας το Windows Hello για επιχειρήσεις.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="5d162-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="5d162-106">**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)**</span><span class="sxs-lookup"><span data-stu-id="5d162-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="5d162-107">Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android.</span><span class="sxs-lookup"><span data-stu-id="5d162-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="5d162-108">Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές.</span><span class="sxs-lookup"><span data-stu-id="5d162-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="5d162-109">Για λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε συσκευές Windows 10, ανατρέξτε στο θέμα Τι είναι το [Διακριτικό κύριας ανανέωσης;](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="5d162-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="5d162-110">**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ**</span><span class="sxs-lookup"><span data-stu-id="5d162-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="5d162-111">Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="5d162-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="5d162-112">Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται στα εξής:</span><span class="sxs-lookup"><span data-stu-id="5d162-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="5d162-113">Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την καταχώρηση (ελέγξτε το KeySignTest κατά την εκτέλεση αναβαθμισμένων)</span><span class="sxs-lookup"><span data-stu-id="5d162-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="5d162-114">Εναλλακτικό αναγνωριστικό σύνδεσης</span><span class="sxs-lookup"><span data-stu-id="5d162-114">Alternate Login ID</span></span>
- <span data-ttu-id="5d162-115">Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε</span><span class="sxs-lookup"><span data-stu-id="5d162-115">HTTP Proxy not found</span></span>

<span data-ttu-id="5d162-116">Για να αντιμετωπίσετε προβλήματα με συσκευές που χρησιμοποιούν την εντολή dsregcmd, ανατρέξτε [στο θέμα Κατάσταση SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="5d162-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
