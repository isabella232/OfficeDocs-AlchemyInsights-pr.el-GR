---
title: 1065 αποδοκιμασία του EOP εξερχόμενων IP διεύθυνση rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934884"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="8d5ca-102">Αποδοκιμασία του EOP εξερχόμενων περιοχές διευθύνσεων IP</span><span class="sxs-lookup"><span data-stu-id="8d5ca-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="8d5ca-p101">Μας έχετε εντοπίσει ένα πιθανό ζήτημα με τον οργανισμό σας που (αν δεν διορθωθεί με την εικοστή Οκτωβρίου 2018), ενδέχεται να καταστρέψετε ροή αλληλογραφίας σας εσωτερικής εγκατάστασης ή εξωτερικούς προορισμούς. Ως γνωστοποιείται προηγουμένως, για να απλοποιήσετε τη Διαχείριση περιοχής διευθύνσεων IP, εμείς συναθροίζετε τις περιοχές διευθύνσεων IP του Exchange Online προστασίας (EOP) που χρησιμοποιούνται για την αποστολή και λήψη ηλεκτρονικού ταχυδρομείου εκτός του Office 365. Την ανάλυση δηλώνει ότι μία ή περισσότερες από τις πηγές εξωτερικής ηλεκτρονικού ταχυδρομείου ή προορισμούς που ορίσατε στο συνδέσεις ροή αλληλογραφίας δεν δέχεται συνδέσεις από το IP διεύθυνση περιοχές εμφανίζονται [εδώ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="8d5ca-106">Ενεργεί πριν από την εικοστή Οκτωβρίου, για τη διασφάλιση αυτών των πηγών και τους προορισμούς θα αποδεχτεί τις συνδέσεις προς και από όλα [δημοσιευτεί διευθύνσεις EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="8d5ca-107">Για περισσότερες πληροφορίες σχετικά με αυτήν την αλλαγή, δείτε καταχωρεί το Κέντρο μηνυμάτων [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ή [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="8d5ca-p102">**Σημείωση**: Εάν χρησιμοποιούσατε προηγουμένως IP ή τη διεύθυνση URL δημοσίευσης μέσω HTML, XML και RSS για ενημερωμένες εκδόσεις του τελικού σημείου, μπορείτε επίσης θα πρέπει να μετεγκαταστήσετε των νέων υπηρεσιών web για την αυτοματοποίηση των αυτοί οι τύποι ενημερώσεων. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [κατηγορίες τελικού σημείου Office 365 και Office 365 IP διεύθυνση και διεύθυνση URL υπηρεσίας web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

