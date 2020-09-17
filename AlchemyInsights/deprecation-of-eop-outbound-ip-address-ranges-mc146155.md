---
title: 1065 αποδοκιμασία της διεύθυνσης IP εξερχομένων του EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806795"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="f17f2-102">Αποδοκιμασία των περιοχών διευθύνσεων IP εξερχομένων του EOP</span><span class="sxs-lookup"><span data-stu-id="f17f2-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="f17f2-103">Εντοπίσαμε ένα πιθανό πρόβλημα με την εταιρεία σας, το οποίο (Εάν δεν διορθωθεί μέχρι τις 26 Οκτωβρίου, 2018) μπορεί να διακόψει τη ροή αλληλογραφίας προς τους εξωτερικούς προορισμούς εσωτερικής εγκατάστασης ή εξωτερικού.</span><span class="sxs-lookup"><span data-stu-id="f17f2-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="f17f2-104">Όπως αναφέρθηκε προηγουμένως, για να απλοποιηθεί η διαχείριση περιοχής διευθύνσεων IP, είμαστε η ενοποίηση των περιοχών διευθύνσεων IP του Exchange Online Protection (EOP) που χρησιμοποιούνται για την αποστολή και λήψη μηνυμάτων ηλεκτρονικού ταχυδρομείου εκτός του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f17f2-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="f17f2-105">Η ανάλυσή μας υποδεικνύει ότι μία ή περισσότερες από τις εξωτερικές πηγές ηλεκτρονικού ταχυδρομείου ή τους προορισμούς που έχετε ρυθμίσει στις γραμμές σύνδεσης ροής αλληλογραφίας δεν δέχονται συνδέσεις από τις περιοχές διευθύνσεων IP που εμφανίζονται [εδώ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="f17f2-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f17f2-106">Ενεργείτε πριν από τις 26 Οκτωβρίου για να εξασφαλίσετε ότι αυτές οι πηγές και οι προορισμοί θα αποδεχθούν συνδέσεις προς και από όλες τις [δημοσιευμένες ΔΙΕΥΘΎΝΣΕΙς IP του EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="f17f2-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f17f2-107">Για περισσότερες πληροφορίες σχετικά με αυτήν την αλλαγή, ανατρέξτε στο θέμα δημοσιεύσεις κέντρου μηνυμάτων [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ή [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="f17f2-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="f17f2-108">**Σημείωση**: Εάν χρησιμοποιήσατε ΠΡΟΗΓΟΥΜΈΝΩς το IP ή τη δημοσίευση διευθύνσεων URL μέσω HTML, XML και RSS για ενημερώσεις τελικών σημείων, θα πρέπει επίσης να κάνετε μετεγκατάσταση στις νέες υπηρεσίες Web για την αυτοματοποίηση αυτών των τύπων ενημερώσεων.</span><span class="sxs-lookup"><span data-stu-id="f17f2-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="f17f2-109">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα κατηγορίες τελικών σημείων του microsoft 365 και διεύθυνση IP του microsoft 365 και υπηρεσία Web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="f17f2-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
