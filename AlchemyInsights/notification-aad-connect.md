---
title: Ειδοποίηση AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036112"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="f7858-102">Ειδοποίηση AAD Connect</span><span class="sxs-lookup"><span data-stu-id="f7858-102">Notification AAD Connect</span></span>

- <span data-ttu-id="f7858-103">Βεβαιωθείτε ότι έχετε εξουσιοδότηση για την εκτέλεση της λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="f7858-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="f7858-104">Οι καθολικοί διαχειριστές έχουν πρόσβαση από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="f7858-104">Global Admins have access by default.</span></span> <span data-ttu-id="f7858-105">Επιπλέον, μπορείτε να χρησιμοποιήσετε τον Έλεγχο πρόσβασης βάσει [ρόλων για να](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) αναθέσετε δικαιώματα καταχώρησης στον Συνεργάτη.</span><span class="sxs-lookup"><span data-stu-id="f7858-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="f7858-106">Βεβαιωθείτε ότι τα απαιτούμενα τελικά σημεία είναι ενεργοποιημένα και δεν αποκλείονται λόγω του τείχους προστασίας.</span><span class="sxs-lookup"><span data-stu-id="f7858-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="f7858-107">Για λεπτομέρειες, ανατρέξτε στις [απαιτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="f7858-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="f7858-108">Η εγγραφή μπορεί να αποτύχει, επειδή η εξερχόμενη επικοινωνία υπόκειται σε έλεγχο SSL από το επίπεδο δικτύου.</span><span class="sxs-lookup"><span data-stu-id="f7858-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="f7858-109">Βεβαιωθείτε ότι έχετε επαληθεύσει τις ρυθμίσεις ειδοποιήσεων για το Azure AD Connect Health και ελέγξτε τη ρύθμιση.</span><span class="sxs-lookup"><span data-stu-id="f7858-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="f7858-110">Για να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους ειδοποιήσεων για τις ειδοποιήσεις υγείας του Azure AD Connect, ανατρέξτε σε αυτόν [τον οδηγό.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="f7858-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="f7858-111">Για να μάθετε περισσότερα σχετικά με την αναφορά συγχρονισμού AAD Connect Health και τον τρόπο λήψης της, ανατρέξτε στην αναφορά [συγχρονισμού επιπέδου αντικειμένου.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="f7858-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="f7858-112">Για να αντιμετωπίσετε προβλήματα με τις ειδοποιήσεις υγείας του [AAD Connect,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ακολουθήστε τον οδηγό αντιμετώπισης προβλημάτων για τις ειδοποιήσεις φρεσκάδας δεδομένων του AAD Connect Health και για συνήθεις ερωτήσεις, ανατρέξτε στο θέμα Συνήθεις ερωτήσεις εγκατάστασης του [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="f7858-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
