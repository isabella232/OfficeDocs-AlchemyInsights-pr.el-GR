---
title: Υπηρεσία σύνδεσης Exchange εσωτερικής εγκατάστασης του Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807649"
---
# <a name="intune-exchange-on-premise-connector"></a>Υπηρεσία σύνδεσης Exchange εσωτερικής εγκατάστασης του Intune

Για λεπτομέρειες σχετικά με τη ρύθμιση της σύνδεσης μεταξύ του Intune και του Exchange που φιλοξενείται εσωτερικής εγκατάστασης, ανατρέξτε στην παρακάτω τεκμηρίωση:

[Ρύθμιση της σύνδεσης του Exchange εσωτερικής εγκατάστασης του Intune στο Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**ΣΥΝΉΘΕΙς ΕΡΩΤΉΣΕΙς**

Ε: εμφανίζεται ένα σφάλμα, όπως "η έκδοση σύνδεσης του Exchange δεν υποστηρίζεται" κατά την προσπάθεια ρύθμισης της σύνδεσης του Exchange. Ποια θα μπορούσε να είναι η αιτία;

Α: ο λογαριασμός που χρησιμοποιείτε έχει άδεια χρήσης κατάλληλα-πρέπει να έχει ενεργή άδεια χρήσης Intune

Ε: είναι δυνατόν να υπάρχουν πολλές γραμμές σύνδεσης του Exchange;

Α: μπορείτε να ρυθμίσετε μόνο μία σύνδεση Exchange ανά μισθωτή του Intune ανά οργανισμό του Exchange. Η γραμμή σύνδεσης μπορεί να εγκατασταθεί μόνο σε ένα διακομιστή σε έναν οργανισμό πολλαπλών διακομιστών Exchange.

Επίσης, δεν μπορείτε να έχετε ρυθμισμένες γραμμές σύνδεσης τόσο για το Exchange εσωτερικής εγκατάστασης όσο και για το Exchange Online που έχει ρυθμιστεί στον ίδιο μισθωτή.

Ε: μπορεί η γραμμή σύνδεσης να χρησιμοποιήσει έναν πίνακα CAS ως σύνδεσή του με το Exchange;

Α: ο καθορισμός ενός πίνακα CAS δεν είναι υποστηριζόμενη ρύθμιση παραμέτρων στη ρύθμιση σύνδεσης. Μόνο ένας διακομιστής πρέπει να καθοριστεί και θα πρέπει να καθορίζεται στο αρχείο ρύθμισης παραμέτρων σύνδεσης που μπορεί να βρεθεί στο

πρόγραμμα data\microsoft\microsoft Intune στη σύνδεση του Exchange εσωτερικής εγκατάστασης \ OnpremiseExchangeConnectorServiceConfiguration.xml

Εντοπίστε την ακόλουθη καταχώρηση ```<ExchangeWebServiceURL />``` και αντικαταστήστε τη διεύθυνση URL με το διακομιστή Exchange.

**Παράδειγμα**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ανατρέξτε στην παρακάτω τεκμηρίωση για πρόσθετες αντιμετώπιση προβλημάτων: [Αντιμετώπιση προβλημάτων της σύνδεσης του Exchange εσωτερικής εγκατάστασης του Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Ενεργοποίηση της λεπτομερούς καταγραφής για τη σύνδεση του Exchange**

1. Ανοίξτε το αρχείο ρύθμισης παραμέτρων ανίχνευσης σύνδεσης του Exchange για επεξεργασία.  
Το αρχείο βρίσκεται στη διεύθυνση:%ProgramData%\Microsoft\Windows του Exchange Intune Connector\TracingConfiguration.xml  

**Παράδειγμα**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Εντοπίστε το TraceSourceLine με το ακόλουθο κλειδί: OnPremisesExchangeConnectorService  
  
3. Αλλαγή της τιμής κόμβου SourceLevel από τις πληροφορίες ActivityTracing (προεπιλογή) σε λεπτομερή ActivityTracing  

**Παράδειγμα**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Επανεκκινήστε την υπηρεσία Microsoft Intune Exchange  
5. Πλήρης συγχρονισμός στην πύλη του Intune μέχρι να ολοκληρωθεί και, στη συνέχεια, αλλάξτε ξανά την XML σε "πληροφορίες ActivityTracing" και επανεκκινήστε την υπηρεσία Microsoft Intune Exchange.  
6. Η θέση των αρχείων καταγραφής είναι: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`