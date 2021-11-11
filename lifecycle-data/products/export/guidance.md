---
title: Eksportveiledning for livssyklusdata
description: Eksporttveiledning for produktlivssyklusinformasjon
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546865"
---
# <a name="lifecycle-data-export-guidance"></a>Eksportveiledning for livssyklusdata
Dette dokumentet beskriver hvordan du bruker produkteksportfilen.

## <a name="query-information"></a>Spørringsinformasjon
I Excel-dokumentet finnes det felt som hjelper deg med å identifisere dataene som er fylt ut i produkttabellen.

### <a name="end-of-support"></a>Dato for støtteavvikling
Verdien for slutten av kundestøtte filtrerer produkter etter enten sluttdatoen for produktet eller sluttdatoen for utgivelsen.

Mulige verdier: Alle (ingen filtre er brukt), år og et område.

### <a name="family"></a>Familie
Familieverdien filtrerer produkter etter det overordnede nivået i hierarkiet som kalles familien.

Mulige verdier: Alle (ingen filtre er brukt), etternavn

### <a name="group"></a>Gruppe
Gruppeverdien filtrerer produkter innenfor det overordnede nivået (familien) til en bestemt gruppe.

Mulige verdier: Alle (ingen filtre er brukt), gruppenavn

## <a name="table-columns"></a>Tabellkolonner
Produkttabellen består av kolonner som definerer produktet, versjonene, utgivelsene og tilhørende støttedatoer.

> [!NOTE]
> Det vil være en rad for hver kombinasjon av produkt, utgave og lansering.

### <a name="product"></a>Produkt
Produktnavnet.

### <a name="edition"></a>Utgave
Utgavekolonnen fylles ut når produktet inneholder utgaver. Når det ikke finnes noen produktutgave, vil dette feltet være tomt.

### <a name="release"></a>Utgivelse
Utgivelseskolonnen fylles ut når produktet inneholder flere utgivelser.
Når produktet bare har én utgivelse, vil dette feltet være tomt.

### <a name="support-policy"></a>Støttepolicy
Dette feltet definerer hvilken støttepolicy produktet følger.

Mulige verdier: [Fast](/lifecycle/policies/fixed), [moderne](/lifecycle/policies/modern), komponent

### <a name="start-date"></a>Startdato
Dato støtten startet for produktet.

### <a name="mainstream-date"></a>Ordinær dato
Når støttepolicyen er **fast** eller **komponent**, er dette datoen produktets vanlige sluttdato.
  
Når støttepolicyen er **moderne**, vil dette være tomt.

### <a name="extended-end-date"></a>Sluttdato for utvidet støtte
Når støttepolicyen er **fast** eller **komponent**, er dette datoen produktets utvidede sluttdato.

Når støttepolicyen er **moderne**, vil dette være tomt.

### <a name="retirement-date"></a>Avviklingsdato
Når støttepolicyen er **fast** eller **komponent**, vil dette være tomt.

Når støttepolicyen er **moderne**, vil dette være produktets avviklingsdato.

### <a name="release-start-date"></a>Startdato for livssyklus
Datoen støtten startet for utgivelsen. Når produktet bare har én utgivelse, vil dette feltet være tomt.
 
### <a name="release-end-date"></a>Utgivelsens sluttdato
Datoen støtten ble avsluttet for utgivelsen.
Når produktet bare har én utgivelse, vil dette feltet være tomt.

### <a name="docs-url"></a>Url for dokumenter
Url-en til utvidet dokumentasjon.
