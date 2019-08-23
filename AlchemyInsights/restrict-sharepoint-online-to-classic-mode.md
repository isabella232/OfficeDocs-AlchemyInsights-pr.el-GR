---
title: Περιορισμός του SharePoint Online σε κλασική προβολή
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551559"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="d981a-102">Περιορισμός του SharePoint Online σε κλασική προβολή</span><span class="sxs-lookup"><span data-stu-id="d981a-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="d981a-103">Ορισμένοι οργανισμοί απαιτούν ακόμη την κλασική εμπειρία σε λειτουργία.</span><span class="sxs-lookup"><span data-stu-id="d981a-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="d981a-104">Ενώ υπάρχουν δεν προβλέπεται να καταργήσετε Κλασική λειτουργία σε ένα λεπτομερές επίπεδο, δεν είναι πλέον δυνατό να περιορίσει μια ολόκληρη εταιρεία (μίσθωσης) σε κλασική λειτουργία για λίστες και βιβλιοθήκες.</span><span class="sxs-lookup"><span data-stu-id="d981a-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="d981a-105">Ο διαχειριστής θα έχει τις ακόλουθες επιλογές για να διαχειριστείτε μεμονωμένες λίστες και βιβλιοθήκες σε κλασική λειτουργία χρησιμοποιώντας κοκκώδη διακόπτες μη συμμετοχής που παρέχουμε με τα παρακάτω επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="d981a-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="d981a-106">συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="d981a-106">site collection</span></span>
- <span data-ttu-id="d981a-107">τοποθεσία</span><span class="sxs-lookup"><span data-stu-id="d981a-107">site</span></span>
- <span data-ttu-id="d981a-108">λίστα</span><span class="sxs-lookup"><span data-stu-id="d981a-108">list</span></span>
- <span data-ttu-id="d981a-109">βιβλιοθήκη</span><span class="sxs-lookup"><span data-stu-id="d981a-109">library</span></span>

<span data-ttu-id="d981a-110">Επιπλέον, οι λίστες που χρησιμοποιούν ορισμένες δυνατότητες και προσαρμογές που δεν υποστηρίζονται από σύγχρονα θα εξακολουθεί να αλλάξει αυτόματα σε κλασική προβολή.</span><span class="sxs-lookup"><span data-stu-id="d981a-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="d981a-111">Ξεκινώντας 1 Απριλίου 2019, τη διαδικασία για να απενεργοποιήσετε το επίπεδο μισθωτών εξαιρεθεί από τη σύγχρονη λίστας και βιβλιοθήκες θα ξεκινήσει και θα συνεχίσει μέχρι τις 31 Μαΐου 2019.</span><span class="sxs-lookup"><span data-stu-id="d981a-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="d981a-112">Οι λίστες και οι βιβλιοθήκες που βρίσκονται σε κλασική λειτουργία λόγω της μη συμμετοχής μισθωτών μετατοπίζεται αυτόματα σε σύγχρονα.</span><span class="sxs-lookup"><span data-stu-id="d981a-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="d981a-113">Εάν χρειάζεστε Κλασική λειτουργία περισσότερες πληροφορίες δείτε [εδώ](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) και οδηγίες τοποθέτησης και Άμεσης λειτουργίας Powershell [εδώ](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) που περιγράφει τις επιλογές και τα εργαλεία που μπορείτε να χρησιμοποιήσετε για να χρησιμοποιήσετε την κλασική λειτουργία εμπειρία σήμερα.</span><span class="sxs-lookup"><span data-stu-id="d981a-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
