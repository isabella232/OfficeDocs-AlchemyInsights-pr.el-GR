---
title: Single-Sign για συνδεδεμένες συσκευές Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405045"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="6e8fa-102">Σύνδεση μίας μόνο υπηρεσίας καταλόγου για συσκευές που είναι συνδεδεμένες στο Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6e8fa-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="6e8fa-103">Εάν έχετε ένα περιβάλλον υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης (AD) και θέλετε να συμμετάσχετε στους υπολογιστές που είναι συνδεδεμένοι με τομέα AD στο Azure AD, μπορείτε να το επιτύχετε αυτό κάνοντας υβριδικό σύνδεσμο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="6e8fa-104">[Τρόπος: Ο σχεδιασμός της υβριδικής](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) εφαρμογής συμμετοχής στο Azure Active Directory σάς παρέχει τα σχετικά βήματα για την υλοποίηση ενός υβριδικού συνδέσμου Azure AD στο περιβάλλον σας.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="6e8fa-105">Ρύθμιση παραμέτρων συσκευών που είναι συνδεδεμένες στο Azure AD για Single-Sign εσωτερικής εγκατάστασης χρησιμοποιώντας το Windows Hello για επιχειρήσεις</span><span class="sxs-lookup"><span data-stu-id="6e8fa-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="6e8fa-106">**Ζητήματα διακριτικού κύριας ανανέωσης (PRT)** Το Διακριτικό κύριας ανανέωσης (PRT) είναι ένα βασικό τεχνούργημα του ελέγχου ταυτότητας Azure AD σε συσκευές Windows 10, Windows Server 2016 και νεότερες εκδόσεις, iOS και Android.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="6e8fa-107">Πρόκειται για ένα Διακριτικό Web JSON (JWT) που έχει εκδοθεί ειδικά για τους μεσίτες διακριτικών πρώτου μέρους της Microsoft για την ενεργοποίηση της μεμονωμένης εισόδου (SSO) σε όλες τις εφαρμογές που χρησιμοποιούνται σε αυτές τις συσκευές.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="6e8fa-108">[Σε τι είναι το Διακριτικό](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)κύριας ανανέωσης; Θα σας παρέχουμε λεπτομέρειες σχετικά με τον τρόπο με τον οποίο εκδίδεται, χρησιμοποιείται και προστατεύεται μια PRT σε συσκευές Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="6e8fa-109">**WamDefaultSet: ΝΑΙ και AzureADPrt: ΝΑΙ** Αυτά τα πεδία υποδεικνύουν εάν ο χρήστης έχει πραγματοποιήσει επιτυχή έλεγχο ταυτότητας στο Azure AD κατά την είσοδο στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="6e8fa-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="6e8fa-110">Εάν οι τιμές είναι **NO,** αυτό μπορεί να οφείλεται:</span><span class="sxs-lookup"><span data-stu-id="6e8fa-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="6e8fa-111">Λάθος κλειδί χώρου αποθήκευσης στο TPM που σχετίζεται με τη συσκευή κατά την εγγραφή (ελέγξτε το KeySignTest ενώ εκτελείται αναβαθμισμένο).</span><span class="sxs-lookup"><span data-stu-id="6e8fa-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="6e8fa-112">Εναλλακτικό αναγνωριστικό σύνδεσης</span><span class="sxs-lookup"><span data-stu-id="6e8fa-112">Alternate Login ID</span></span>
- <span data-ttu-id="6e8fa-113">Ο διακομιστής μεσολάβησης HTTP δεν βρέθηκε</span><span class="sxs-lookup"><span data-stu-id="6e8fa-113">HTTP Proxy not found</span></span>

<span data-ttu-id="6e8fa-114">Αντιμετώπιση προβλημάτων συσκευών με χρήση της εντολής dsregcmd - [Κατάσταση SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="6e8fa-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
