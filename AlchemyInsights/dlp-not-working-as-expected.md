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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707810"
---
# <a name="dlp-not-working-as-expected"></a>Η DLP δεν λειτουργεί όπως αναμένεται

**Σημαντικό**: Σε αυτή την πρωτοφανή χρονική στιγμή, θα πρέπει να διασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες στον μέγιστο βαθμό. Επισκεφτείτε το θέμα [Προσωρινές ρυθμίσεις δυνατοτήτων του SharePoint Online](https://aka.ms/ODSPAdjustments) για περισσότερες πληροφορίες.

 **Ρύθμιση DLP**

Αντιμετωπίζετε προβλήματα με την **Αποτροπή απώλειας δεδομένων (DLP)** στο Office 365 και δεν λειτουργεί όπως αναμένεται; Σε αυτήν την περίπτωση, βεβαιωθείτε ότι η πολιτική **DLP** έχει ρυθμιστεί σωστά και ότι τα δεδομένα σας περιέχουν αυτό που αναζητά η πολιτική **DLP** κατά την αξιολόγηση.
  
Οι πολιτικές DLP σάς επιτρέπουν να αναγνωρίζετε και να προστατεύετε ευαίσθητες πληροφορίες στον οργανισμό σας. Για να ρυθμίσετε πολιτικές DLP, χρησιμοποιήστε τις πληροφορίες [εδώ.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Ποιες πολιτικές DLP πρέπει να αναζητήσουν**
  
Όταν χρησιμοποιείτε τους **ενσωματωμένους τύπους** ευαίσθητων πληροφοριών στα κέντρα ασφάλειας και συμμόρφωσης, οι πολιτικές DLP αναζητήστε συγκεκριμένα μοτίβα και στοιχεία κατά τον εντοπισμό αυτών των ευαίσθητων τύπων.
  
- **Ενσωματωμένοι τύποι ευαίσθητων πληροφοριών**

    Για πληροφορίες σχετικά με τους ενσωματωμένους τύπους ευαίσθητων πληροφοριών και τι αναζητά μια πολιτική DLP κατά τον εντοπισμό του τύπου "Ευαίσθητα", ανατρέξτε στο θέμα: Τι αναζητά ο τύπος [ευαίσθητων πληροφοριών.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Προσαρμοσμένοι τύποι ευαίσθητων πληροφοριών**

    Εάν προσπαθείτε να δημιουργήσετε προσαρμοσμένους τύπους ευαίσθητων πληροφοριών, χρησιμοποιήστε το παρακάτω άρθρο για πληροφορίες σχετικά με τον τρόπο δημιουργίας ενός προσαρμοσμένου ευαίσθητου τύπου: Δημιουργία προσαρμοσμένου [τύπου ευαίσθητων πληροφοριών.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Δοκιμή πολιτικής DLP**

Για να ελέγξετε τα δεδομένα σας με έναν  ενσωματωμένο ή προσαρμοσμένο τύπο ευαίσθητων πληροφοριών, χρησιμοποιήστε την επιλογή "Τύπος δοκιμής" στην περιοχή **"Τύποι**  >  **ευαίσθητων πληροφοριών".** Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Δοκιμή προσαρμοσμένων τύπων ευαίσθητων πληροφοριών".](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Αναφορές**
  
- Αποκτήστε ευαίσθητα δεδομένα με [αναφορές DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Δείτε συγκεκριμένες λεπτομέρειες του συμβάντος με μια [αναφορά περιστατικού.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
