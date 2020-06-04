---
title: Πώς να ενεργοποιήσετε απρόσκοπτη SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36663860"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="20f40-102">Πώς να ενεργοποιήσετε απρόσκοπτη SSO</span><span class="sxs-lookup"><span data-stu-id="20f40-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="20f40-103">Ενεργοποίηση απρόσκοπτου SSO μέσω [της σύνδεσης Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="20f40-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="20f40-104">Εάν κάνετε μια νέα εγκατάσταση του Azure AD Connect, επιλέξτε την [προσαρμοσμένη διαδρομή εγκατάστασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="20f40-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="20f40-105">Στη σελίδα **Είσοδος χρήστη,** ενεργοποιήστε την επιλογή **Ενεργοποίηση μεμονωμένης σύνδεσης.**</span><span class="sxs-lookup"><span data-stu-id="20f40-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="20f40-106">Για να επαληθεύσετε ότι έχετε ενεργοποιήσει σωστά το SSO χωρίς ραφή:</span><span class="sxs-lookup"><span data-stu-id="20f40-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="20f40-107">Πραγματοποιήστε είσοδο στο κέντρο διαχείρισης της [υπηρεσίας καταλόγου Active Directory Azure](https://aad.portal.azure.com) ως καθολικός διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="20f40-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="20f40-108">Επιλέξτε **Υπηρεσία καταλόγου Active Directory Azure** στο αριστερό τμήμα παραθύρου.</span><span class="sxs-lookup"><span data-stu-id="20f40-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="20f40-109">Βεβαιωθείτε ότι η καθολική σύνδεση χωρίς σύνδεση είναι **ενεργοποιημένη**.</span><span class="sxs-lookup"><span data-stu-id="20f40-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="20f40-110">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [Μεμονωμένη σύνδεση της υπηρεσίας καταλόγου Active Directory Azure χωρίς ραφή: Γρήγορη εκκίνηση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="20f40-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  