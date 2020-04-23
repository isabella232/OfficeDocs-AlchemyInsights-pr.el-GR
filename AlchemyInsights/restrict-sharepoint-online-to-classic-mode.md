---
title: Περιορισμός του SharePoint Online σε κλασική λειτουργία
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742469"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="71bc9-102">Περιορισμός του SharePoint Online σε κλασική λειτουργία</span><span class="sxs-lookup"><span data-stu-id="71bc9-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="71bc9-103">Ορισμένοι οργανισμοί εξακολουθούν να απαιτούν την εμπειρία κλασικής λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="71bc9-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="71bc9-104">Παρόλο που δεν υπάρχουν σχέδια κατάργησης της κλασικής λειτουργίας σε επίπεδο λεπτομέρειας, δεν είναι πλέον δυνατό να περιορίσετε έναν ολόκληρο οργανισμό (μισθωτή) σε κλασική λειτουργία για λίστες και βιβλιοθήκες.</span><span class="sxs-lookup"><span data-stu-id="71bc9-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="71bc9-105">Ο διαχειριστής θα έχει τις ακόλουθες επιλογές για τη διαχείριση μεμονωμένων λιστών και βιβλιοθηκών σε κλασική λειτουργία χρησιμοποιώντας λεπτομερείς διακόπτες εξαίρεσης που παρέχουμε στα ακόλουθα επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="71bc9-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="71bc9-106">συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="71bc9-106">site collection</span></span>
- <span data-ttu-id="71bc9-107">Τοποθεσία</span><span class="sxs-lookup"><span data-stu-id="71bc9-107">site</span></span>
- <span data-ttu-id="71bc9-108">Λίστα</span><span class="sxs-lookup"><span data-stu-id="71bc9-108">list</span></span>
- <span data-ttu-id="71bc9-109">Βιβλιοθήκη</span><span class="sxs-lookup"><span data-stu-id="71bc9-109">library</span></span>

<span data-ttu-id="71bc9-110">Επιπλέον, οι λίστες που χρησιμοποιούν ορισμένες δυνατότητες και προσαρμογές που δεν υποστηρίζονται από σύγχρονες θα εξακολουθούν να μεταπηδούν αυτόματα σε κλασική λειτουργία.</span><span class="sxs-lookup"><span data-stu-id="71bc9-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="71bc9-111">Από την 1η Απριλίου 2019, η διαδικασία απενεργοποίησης του επιπέδου μισθωτή θα εξαιρεθεί από τη σύγχρονη λίστα και οι βιβλιοθήκες θα ξεκινήσει και θα συνεχιστεί έως τις 31 Μαΐου 2019.</span><span class="sxs-lookup"><span data-stu-id="71bc9-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="71bc9-112">Οι λίστες και οι βιβλιοθήκες που βρίσκονται σε κλασική λειτουργία ως αποτέλεσμα της εξαίρεσης μισθωτή θα μετατοπιστούν αυτόματα στη σύγχρονη.</span><span class="sxs-lookup"><span data-stu-id="71bc9-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="71bc9-113">Εάν χρειάζεστε κλασική λειτουργία, ανατρέξτε σε περισσότερες πληροφορίες [εδώ](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) και οδηγίες PnP Powershell [εδώ](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) που περιγράφει τις επιλογές και τα εργαλεία που μπορείτε να χρησιμοποιήσετε σήμερα για να χρησιμοποιήσετε την κλασική εμπειρία λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="71bc9-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
