---
title: EndPoint Manager - Γραμμές βάσης ασφάλειας
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923554"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Γραμμές βάσης ασφάλειας

Οι γραμμές βάσης ασφαλείας είναι προκαθορισμένες ομάδες ρυθμίσεων των Windows που σας βοηθούν να εφαρμόσετε τις ρυθμίσεις ασφαλείας που συνιστώνται από τις σχετικές ομάδες ασφαλείας. Αυτές οι γραμμές βάσης μπορούν να προσαρμοστούν ώστε να παρέχουν μόνο τις ρυθμίσεις και τις τιμές που θέλετε. Για περισσότερες πληροφορίες σχετικά με τις γραμμές βάσης ασφαλείας, ανατρέξτε στο θέμα [Χρήση γραμμών βάσης ασφαλείας για τη ρύθμιση παραμέτρων των συσκευών Windows 10 στο Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Υπάρχουν προς το παρόν γραμμές βάσης για αυτά τα προϊόντα:

- Ρυθμίσεις ασφαλείας Windows MDM
- Microsoft Defender για την ασφάλεια του EndPoint
- Microsoft Edge

Κάθε μία από τις γραμμές βάσης ενημερώνεται περιοδικά και κυκλοφορεί με προοδευτικές εκδόσεις. Κάθε έκδοση προσθέτει ή καταργεί ρυθμίσεις από την προηγούμενη έκδοση, για να διασφαλιστεί ότι η γραμμή βάσης πληροί τις τρέχουσες οδηγίες. Η κονσόλα γραμμών βάσης ασφαλείας στην Ασφάλεια Endpoint επιτρέπει τη σύγκριση διαφορετικών εκδόσεων, κάνοντας ορατές τις αλλαγές από έκδοση σε έκδοση.

Για οδηγίες σχετικά με τον τρόπο πιο αποτελεσματικής αλλαγής της έκδοσης της γραμμής βάσης που αναπτύσσεται, ανατρέξτε στο θέμα [Διαχείριση των προφίλ γραμμών βάσης ασφαλείας στο Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Μετά την ανάπτυξη μιας γραμμής βάσης ασφαλείας, μπορείτε να παρακολουθείτε την κατάσταση της ανάπτυξης και να αναθεωρείτε τις ρυθμίσεις ανά συσκευή.

Επειδή οι γραμμές βάσης ασφαλείας περιέχουν πολλές ρυθμίσεις, είναι σημαντικό να εξετάσετε τις αλλαγές ρύθμισης παραμέτρων και να εκτελέσετε δοκιμές, για να βεβαιωθείτε ότι όλες οι ρυθμίσεις είναι κατάλληλες για τις συσκευές και τις επιχειρηματικές ανάγκες σας.

**Σημείωση:** Τα δεδομένα αναφοράς για τις γραμμές βάσης ενδέχεται να χρειαστεί έως και 24 ώρες για να εμφανιστούν από την αρχική ανάπτυξη σε μια συσκευή και έως 6 ώρες για περαιτέρω ενημερώσεις. 

Η πιο συνηθισμένη αιτία της μη εφαρμογής μιας ρύθμισης γραμμής βάσης είναι επειδή η ίδια ρύθμιση χρησιμοποιείται σε διαφορετικό προφίλ. Αυτό το σενάριο μπορεί να διερευνηθεί για συγκεκριμένη συσκευή, επιλέγοντας αυτή τη συσκευή από τον κόμβο "Κατάσταση συσκευής" του προφίλ γραμμής βάσης ασφάλειας. Για λεπτομέρειες, ανατρέξτε στο θέμα [Επίλυση διενέξεων για γραμμές βάσης](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).