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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30955989"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="7ceec-102">Περιορισμός του SharePoint Online σε κλασική προβολή</span><span class="sxs-lookup"><span data-stu-id="7ceec-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="7ceec-103">Ορισμένοι οργανισμοί απαιτούν ακόμη την κλασική εμπειρία σε λειτουργία.</span><span class="sxs-lookup"><span data-stu-id="7ceec-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="7ceec-104">Ενώ υπάρχουν δεν προβλέπεται να καταργήσετε Κλασική λειτουργία σε ένα λεπτομερές επίπεδο, ξεκινώντας Απριλίου 1,2019, δεν θα είναι πλέον δυνατό να περιορίσει μια ολόκληρη εταιρεία (μίσθωσης) σε κλασική λειτουργία για λίστες και βιβλιοθήκες.</span><span class="sxs-lookup"><span data-stu-id="7ceec-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="7ceec-105">Ο διαχειριστής θα έχει τις ακόλουθες επιλογές για να διαχειριστείτε μεμονωμένες λίστες και βιβλιοθήκες σε κλασική λειτουργία χρησιμοποιώντας κοκκώδη διακόπτες μη συμμετοχής που παρέχουμε με τα παρακάτω επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="7ceec-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="7ceec-106">συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="7ceec-106">site collection</span></span>
- <span data-ttu-id="7ceec-107">τοποθεσία</span><span class="sxs-lookup"><span data-stu-id="7ceec-107">site</span></span>
- <span data-ttu-id="7ceec-108">λίστα</span><span class="sxs-lookup"><span data-stu-id="7ceec-108">list</span></span>
- <span data-ttu-id="7ceec-109">βιβλιοθήκη</span><span class="sxs-lookup"><span data-stu-id="7ceec-109">library</span></span>

<span data-ttu-id="7ceec-110">Επιπλέον, οι λίστες που χρησιμοποιούν ορισμένες δυνατότητες και προσαρμογές που δεν υποστηρίζονται από σύγχρονα θα εξακολουθεί να αλλάξει αυτόματα σε κλασική προβολή.</span><span class="sxs-lookup"><span data-stu-id="7ceec-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="7ceec-111">Μετά από την 1η Απριλίου, λίστες και βιβλιοθήκες που βρίσκονται σε κλασική λειτουργία λόγω της μη συμμετοχής μισθωτών αυτόματα γίνεται στο επίπεδο τοποθεσίας και επίπεδο λίστας.</span><span class="sxs-lookup"><span data-stu-id="7ceec-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="7ceec-112">Εάν χρειάζεστε Κλασική λειτουργία, ανατρέξτε εδώ περισσότερες πληροφορίες και οδηγίες τοποθέτησης και Άμεσης λειτουργίας Powershell εδώ περιγράφει επιλογές και τα εργαλεία μπορείτε να χρησιμοποιήσετε σήμερα για την προετοιμασία για την κατάργηση της μίσθωσης επιπέδου μη συμμετοχής την 1η Απριλίου.</span><span class="sxs-lookup"><span data-stu-id="7ceec-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>