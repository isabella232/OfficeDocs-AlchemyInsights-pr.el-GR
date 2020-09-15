---
title: Η τεχνολογία DLP δεν λειτουργεί όπως αναμένεται
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679693"
---
# <a name="dlp-not-working-as-expected"></a>Η τεχνολογία DLP δεν λειτουργεί όπως αναμένεται

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

 **Ρύθμιση DLP**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** στο Office 365 που δεν λειτουργεί όπως αναμένεται; Εάν Ναι, βεβαιωθείτε ότι η **πολιτική DLP** έχει ρυθμιστεί σωστά και ότι τα δεδομένα σας περιέχουν αυτό που αναζητά η **πολιτική DLP** όταν αξιολογείται.
  
Οι πολιτικές DLP σάς επιτρέπουν να εντοπίζετε και να προστατεύετε ευαίσθητες πληροφορίες στον οργανισμό σας. Για να ρυθμίσετε τις πολιτικές DLP, χρησιμοποιήστε τις πληροφορίες [εδώ](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Τι αναζητούν οι πολιτικές DLP**
  
Όταν χρησιμοποιείτε τους **ενσωματωμένους τύπους ευαίσθητων πληροφοριών** στα κέντρα ασφάλειας και συμμόρφωσης, οι πολιτικές DLP αναζητούν συγκεκριμένα μοτίβα και στοιχεία κατά τον εντοπισμό αυτών των ευαίσθητων τύπων.
  
- **Ενσωματωμένοι ευαίσθητοι τύποι πληροφοριών**

    Για πληροφορίες σχετικά με τους ενσωματωμένους ευαίσθητους τύπους και τι αναζητά μια πολιτική DLP κατά τον εντοπισμό του ευαίσθητου τύπου, ανατρέξτε στο θέμα: [Τι αναζητούν οι τύποι ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Προσαρμοσμένοι τύποι ευαίσθητων πληροφοριών**

    Εάν προσπαθείτε να δημιουργήσετε προσαρμοσμένους τύπους ευαίσθητων πληροφοριών, χρησιμοποιήστε το ακόλουθο άρθρο για πληροφορίες σχετικά με τον τρόπο δημιουργίας ενός προσαρμοσμένου ευαίσθητου τύπου: [Δημιουργία προσαρμοσμένου τύπου ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Δοκιμή μιας πολιτικής DLP**

Για να ελέγξετε τα δεδομένα σας με έναν ενσωματωμένο ή προσαρμοσμένο ευαίσθητο τύπο πληροφοριών, χρησιμοποιήστε την επιλογή **Έλεγχος τύπου** στην περιοχή **ταξινομήσεις**  >  **ευαίσθητων τύπων**πληροφοριών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [δοκιμή τύπων προσαρμοσμένων ευαίσθητων πληροφοριών](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Αναφορές**
  
- Λήψη ευαίσθητων ιδεών δεδομένων με τις [αναφορές DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Δείτε συγκεκριμένες λεπτομέρειες για το συμβάν με μια [αναφορά περιστατικού](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
