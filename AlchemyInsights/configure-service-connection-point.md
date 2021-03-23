---
title: Ρύθμιση παραμέτρων σημείου σύνδεσης υπηρεσίας (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036141"
---
# <a name="configure-service-connection-point-scp"></a>Ρύθμιση παραμέτρων σημείου σύνδεσης υπηρεσίας (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Αιτία:** Δεν είναι δυνατή η ανάγνωση του αντικειμένου SCP και η λήψη των πληροφοριών μισθωτή Azure AD
- **Επίλυση:** Ανατρέξτε στην ενότητα "Ρύθμιση [παραμέτρων σημείου σύνδεσης υπηρεσίας"](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Σχέδιο δράσης**

- Ελέγξτε εάν η συσκευή έχει λάβει το GPO για την ελεγχόμενη επικύρωση.
- Βεβαιωθείτε ότι το GPO έχει δημιουργήσει τα κλειδιά μητρώου.
- Βεβαιωθείτε ότι έχετε δημιουργήσει 2 κλειδιά με το αναγνωριστικό καταλόγου και τον τομέα onmicrosoft.

**Ρύθμιση παραμέτρων μητρώου από την πλευρά του προγράμματος-πελάτη για SCP**

Χρησιμοποιήστε το παρακάτω παράδειγμα για να δημιουργήσετε ένα αντικείμενο πολιτικής ομάδας (GPO) για να αναπτύξετε μια ρύθμιση μητρώου που ρυθμίζει τις παραμέτρους μιας καταχώρησης SCP στο μητρώο των συσκευών σας.

1. Ανοίξτε μια κονσόλα διαχείρισης πολιτικής ομάδας και δημιουργήστε ένα νέο GPO στον τομέα σας.
     - Δώστε ένα όνομα στο GPO που μόλις δημιουργήσατε (για παράδειγμα, ClientSideSCP)

2. Επεξεργαστείτε το GPO και εντοπίστε την ακόλουθη διαδρομή: Ρυθμίσεις **παραμέτρων υπολογιστή > προτιμήσεις > ρυθμίσεις των Windows > Μητρώο.**

3. Κάντε δεξί κλικ στο **Μητρώο και** επιλέξτε **"Νέο > μητρώου".**

4. Στην καρτέλα **"Γενικά",** ρυθμίστε τις παραμέτρους για τα εξής:
  
- **Ενέργεια:** Ενημέρωση
    
- **Ομάδα**: HKEY_LOCAL_MACHINE
    
- **Διαδρομή κλειδιού:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Όνομα τιμής:** TenantId
    
- **Τύπος τιμής:** REG_SZ
    
- **Δεδομένα τιμής:** Το αναγνωριστικό GUID ή καταλόγου της παρουσίας azure AD (Αυτή η τιμή μπορεί να βρεθεί στην πύλη **Azure > Azure Active Directory > Ιδιότητες > αναγνωριστικό καταλόγου)**
 
- Κάντε κλικ στο κουμπί **OK**.
 
5. Κάντε δεξί κλικ στο **Μητρώο και** επιλέξτε **"Νέο > μητρώου".**

6. Στην καρτέλα **"Γενικά",** ρυθμίστε τις παραμέτρους για τα εξής:
  
- **Ενέργεια:** Ενημέρωση
    
- **Ομάδα**: HKEY_LOCAL_MACHINE
    
- **Διαδρομή κλειδιού:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Όνομα τιμής:** Όνομα μισθωτή
    
- **Τύπος τιμής:** REG_SZ
    
- **Δεδομένα τιμών:** Το επαληθευμένο όνομα τομέα σας, εάν χρησιμοποιείτε ομόσπονδο περιβάλλον, όπως AD FS. Το επαληθευμένο όνομα τομέα ή το onmicrosoft.com τομέα σας (για παράδειγμα, contoso.onmicrosoft).com εάν χρησιμοποιείτε διαχειριζόμενο περιβάλλον

- Κάντε κλικ στο κουμπί **OK**.

7. Κλείστε το πρόγραμμα επεξεργασίας για το GPO που μόλις δημιουργήσατε.

8. Συνδέστε το νέο GPO με την επιθυμητή OU που περιέχει υπολογιστές που συνδέονται με τομέα και ανήκουν στον ελεγχόμενο πληθυσμό της συνάθροισης.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ελεγχόμενη επικύρωση υβριδικού συνδέσμου Azure AD - Azure AD | Συσκευές που είναι συνδεδεμένες](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) στο Azure Active Directory και  [αντιμετώπιση προβλημάτων με υβριδικές συσκευές | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









