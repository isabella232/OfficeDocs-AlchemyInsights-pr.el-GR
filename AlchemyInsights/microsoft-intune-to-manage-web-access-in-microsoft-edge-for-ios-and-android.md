---
title: Χρήση του Microsoft Intune για τη διαχείριση της πρόσβασης στο Web στον Microsoft Edge για iOS και Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989673"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="cb5e2-102">Χρήση του Microsoft Intune για τη διαχείριση της πρόσβασης στο Web στον Microsoft Edge για iOS και Android</span><span class="sxs-lookup"><span data-stu-id="cb5e2-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="cb5e2-103">Ο Microsoft Edge για iOS και Android επιτρέπει σε ένα χρήστη να περιηγηθεί στο web από πολλά, εντελώς ξεχωριστά προφίλ.</span><span class="sxs-lookup"><span data-stu-id="cb5e2-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="cb5e2-104">Οι ευρύτερες δυνατότητες προστασίας για τα δεδομένα του Microsoft 365 γίνονται διαθέσιμες όταν εγγράφεστε στην οικογένεια προγραμμάτων Enterprise Mobility + Security, η οποία περιλαμβάνει τις δυνατότητες Microsoft Intune και Azure Active Directory Premium, όπως η πρόσβαση υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="cb5e2-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="cb5e2-105">Τουλάχιστον, θα θέλετε να αναπτύξετε μια πολιτική πρόσβασης υπό όρους που (1) επιτρέπει στους χρήστες να συνδέονται από κινητές συσκευές στον Microsoft Edge για iOS και Android και ότι (2) εφαρμόζει μια πολιτική προστασίας εφαρμογών του Microsoft Intune που παρέχει μια προστατευμένη εμπειρία περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="cb5e2-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="cb5e2-106">Για να κατανοήσετε πώς μπορείτε να χρησιμοποιήσετε την πρόσβαση υπό όρους και τις πολιτικές, ανατρέξτε στα θέμα:</span><span class="sxs-lookup"><span data-stu-id="cb5e2-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="cb5e2-107">Εφαρμογή πολιτικών πρόσβασης υπό όρους της υπηρεσίας καταλόγου Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cb5e2-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="cb5e2-108">Δημιουργία πολιτικών προστασίας εφαρμογών του Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cb5e2-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="cb5e2-109">Χρήση μεμονωμένης σύνδεσης για εφαρμογές Web που είναι συνδεδεμένες με το Azure Active Directory σε προγράμματα περιήγησης που προστατεύονται με πολιτική</span><span class="sxs-lookup"><span data-stu-id="cb5e2-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="cb5e2-110">Χρήση της ρύθμισης παραμέτρων εφαρμογής για τη διαχείριση της εμπειρίας περιήγησης</span><span class="sxs-lookup"><span data-stu-id="cb5e2-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="cb5e2-111">Να επιτρέπεται η χρήση μόνο των λογαριασμών εργασίας και σχολείου</span><span class="sxs-lookup"><span data-stu-id="cb5e2-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="cb5e2-112">Ανάπτυξη γενικών πολιτικών ρύθμισης παραμέτρων εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="cb5e2-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="cb5e2-113">Ανάπτυξη πολιτικών ρύθμισης παραμέτρων εφαρμογής για την προστασία δεδομένων</span><span class="sxs-lookup"><span data-stu-id="cb5e2-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="cb5e2-114">Χρήση της Διαχείρισης τελικού σημείου της Microsoft για την ανάπτυξη πολιτικών ρύθμισης παραμέτρων εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="cb5e2-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="cb5e2-115">Για να μάθετε πώς μπορείτε να αποκτήσετε πρόσβαση σε διαχειριζόμενα αρχεία καταγραφής εφαρμογών, ανατρέξτε στο θέμα Χρήση του [Microsoft Edge για iOS και Android για πρόσβαση σε διαχειριζόμενα αρχεία καταγραφής εφαρμογών.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="cb5e2-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
