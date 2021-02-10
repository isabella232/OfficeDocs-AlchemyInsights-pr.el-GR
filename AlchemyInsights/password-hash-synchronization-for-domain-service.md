---
title: Συγχρονισμός hash κωδικού πρόσβασης για την υπηρεσία τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177491"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="bd343-102">Συγχρονισμός hash κωδικού πρόσβασης για την υπηρεσία τομέα</span><span class="sxs-lookup"><span data-stu-id="bd343-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="bd343-103">**Εάν η παρουσία azure AD DS σάς ζητά να ενεργοποιήσετε το συγχρονισμό hash κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="bd343-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="bd343-104">Αντιμετωπίζετε ένα σενάριο στο οποίο εκτελείτε ένα υβριδικό περιβάλλον με χρήστες που συγχρονίζονται από ένα περιβάλλον υπηρεσιών τομέα Azure Active Directory (AD DS) εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="bd343-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="bd343-105">Αυτό το σενάριο αντιμετωπίζεται παρά το γεγονός ότι έχετε συγχρονισμό hash κωδικού πρόσβασης από τις υπηρεσίες AD DS εσωτερικής εγκατάστασης στο μισθωτή azure AD.</span><span class="sxs-lookup"><span data-stu-id="bd343-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="bd343-106">**Αιτία**</span><span class="sxs-lookup"><span data-stu-id="bd343-106">**Cause**</span></span>

<span data-ttu-id="bd343-107">Αυτό συμβαίνει επειδή το Azure AD Connect από προεπιλογή δεν συγχρονίζει hashes κωδικού πρόσβασης LAN Manager νέας τεχνολογίας παλαιού τύπου (NTLM) και Kerberos που είναι απαραίτητοι για το Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="bd343-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="bd343-108">**Λύση**</span><span class="sxs-lookup"><span data-stu-id="bd343-108">**Workaround**</span></span> 

<span data-ttu-id="bd343-109">Θα πρέπει να ρυθμίσετε τις παραμέτρους του Azure AD Connect για να συγχρονίσετε αυτούς τους hashes κωδικού πρόσβασης που απαιτούνται για τον έλεγχο ταυτότητας NTLM και Kerberos.</span><span class="sxs-lookup"><span data-stu-id="bd343-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="bd343-110">Αφού ρυθμιστούν οι παράμετροι του Azure AD Connect, ένα συμβάν δημιουργίας ή αλλαγής κωδικού πρόσβασης εσωτερικής εγκατάστασης συγχρονίζει επίσης τον κωδικό πρόσβασης παλαιού τύπου στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bd343-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="bd343-111">Ανατρέξτε [εδώ για](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) περισσότερες πληροφορίες σχετικά με αυτό το θέμα και για οδηγίες σχετικά με τον τρόπο ενεργοποίησης του συγχρονισμού κωδικών πρόσβασης σε υβριδικά περιβάλλοντα Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="bd343-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>