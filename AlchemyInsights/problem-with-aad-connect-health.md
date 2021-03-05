---
title: Πρόβλημα με το AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481467"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="37de1-102">Πρόβλημα με το AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="37de1-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="37de1-103">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για την εκτέλεση της λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="37de1-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="37de1-104">Οι καθολικοί διαχειριστές έχουν πρόσβαση από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="37de1-104">Global Admins have access by default.</span></span> <span data-ttu-id="37de1-105">Επιπλέον, μπορείτε να χρησιμοποιήσετε τον Έλεγχο πρόσβασης βάσει [ρόλων για να](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) αναθέσετε δικαιώματα καταχώρησης στον Συνεργάτη.</span><span class="sxs-lookup"><span data-stu-id="37de1-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="37de1-106">Βεβαιωθείτε ότι τα απαιτούμενα τελικά σημεία είναι ενεργοποιημένα και δεν έχουν αποκλειστεί λόγω του τείχους προστασίας.</span><span class="sxs-lookup"><span data-stu-id="37de1-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="37de1-107">Για λεπτομέρειες, ανατρέξτε στις [απαιτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="37de1-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="37de1-108">Η καταχώρηση μπορεί να αποτύχει λόγω του ότι η εξερχόμενη επικοινωνία υπόκειται σε έλεγχο SSL από το επίπεδο δικτύου.</span><span class="sxs-lookup"><span data-stu-id="37de1-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="37de1-109">Βεβαιωθείτε ότι έχετε επαληθεύσει τις ρυθμίσεις ειδοποιήσεων για το Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="37de1-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="37de1-110">Ελέγξτε τη ρυθμίσεών σας.</span><span class="sxs-lookup"><span data-stu-id="37de1-110">Please review your setting.</span></span> <span data-ttu-id="37de1-111">Αυτός ο [οδηγός μπορεί](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) να σας βοηθήσει να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους ειδοποιήσεων για ειδοποιήσεις σχετικά με την κατάσταση του Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="37de1-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="37de1-112">Για να μάθετε περισσότερα σχετικά με την αναφορά συγχρονισμού της υγείας του AAD Connect και τον τρόπο λήψης της, ανατρέξτε στην [αναφορά συγχρονισμού επιπέδου αντικειμένου.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="37de1-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="37de1-113">Για την αντιμετώπιση προβλημάτων με τις ειδοποιήσεις υγείας του AAD Connect, ακολουθήστε τον οδηγό αντιμετώπισης προβλημάτων για τις ειδοποιήσεις πιο πρόσφατα δεδομένα του [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) και για συνήθεις ερωτήσεις, ανατρέξτε στις συνήθεις ερωτήσεις σχετικά με την εγκατάσταση του [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="37de1-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
