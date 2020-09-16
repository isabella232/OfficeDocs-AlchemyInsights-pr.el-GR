---
title: Περιορισμός του SharePoint Online σε κλασική λειτουργία
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751422"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="942f3-102">Περιορισμός του SharePoint Online σε κλασική λειτουργία</span><span class="sxs-lookup"><span data-stu-id="942f3-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="942f3-103">Ορισμένες εταιρείες εξακολουθούν να απαιτούν την κλασική εμπειρία λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="942f3-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="942f3-104">Παρόλο που δεν υπάρχουν σχέδια για την κατάργηση της κλασικής λειτουργίας σε κοκκώδη επίπεδο, δεν είναι πλέον δυνατός ο περιορισμός μιας ολόκληρης εταιρείας (μισθωτής) σε κλασική λειτουργία για λίστες και βιβλιοθήκες.</span><span class="sxs-lookup"><span data-stu-id="942f3-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="942f3-105">Ο διαχειριστής θα έχει τις ακόλουθες επιλογές για τη διαχείριση μεμονωμένων λιστών και βιβλιοθηκών στην κλασική λειτουργία, χρησιμοποιώντας τους αναλυτικούς διακόπτες εξαίρεσης που παρέχουμε στα παρακάτω επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="942f3-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="942f3-106">συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="942f3-106">site collection</span></span>
- <span data-ttu-id="942f3-107">τοποθεσία</span><span class="sxs-lookup"><span data-stu-id="942f3-107">site</span></span>
- <span data-ttu-id="942f3-108">λίστα</span><span class="sxs-lookup"><span data-stu-id="942f3-108">list</span></span>
- <span data-ttu-id="942f3-109">Βιβλιοθήκη</span><span class="sxs-lookup"><span data-stu-id="942f3-109">library</span></span>

<span data-ttu-id="942f3-110">Επιπλέον, οι λίστες που χρησιμοποιούν ορισμένες δυνατότητες και προσαρμογές που δεν υποστηρίζονται από τη σύγχρονη θα εξακολουθούν να μετατρέπονται αυτόματα σε κλασική λειτουργία.</span><span class="sxs-lookup"><span data-stu-id="942f3-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="942f3-111">Από την 1η Απριλίου του 2019, η διαδικασία απενεργοποίησης του επιπέδου μισθωτών από τη σύγχρονη λίστα και βιβλιοθήκες θα ξεκινήσει και θα συνεχιστεί μέχρι τις 31 Μαΐου 2019.</span><span class="sxs-lookup"><span data-stu-id="942f3-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="942f3-112">Οι λίστες και οι βιβλιοθήκες που βρίσκονται στην κλασική λειτουργία, ως αποτέλεσμα της εξαίρεσης του μισθωτή, θα μετατοπιστούν αυτόματα στη σύγχρονη μορφή.</span><span class="sxs-lookup"><span data-stu-id="942f3-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="942f3-113">Εάν χρειάζεστε κλασική λειτουργία, ανατρέξτε [εδώ](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) για περισσότερες πληροφορίες και οδηγίες για την εφαρμογή PNP PowerShell [εδώ](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) που περιγράφουν τις επιλογές και τα εργαλεία που μπορείτε να χρησιμοποιήσετε σήμερα για να χρησιμοποιήσετε την κλασική εμπειρία λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="942f3-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
