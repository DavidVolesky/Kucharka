---
layout: default
title: Drinky
nav_order: 2
---

# Drinky

<button onclick="toggleUnits()" id="unitToggle" style="padding: 10px 20px; cursor: pointer; border-radius: 5px; border: 1px solid #ccc; background: #f9f9f9; font-weight: bold;">
  Přepnout na Oz
</button>

<script>
let isOz = false;
function toggleUnits() {
  const elements = document.querySelectorAll('.unit-ml');
  isOz = !isOz;
  
  elements.forEach(el => {
    let val = parseFloat(el.getAttribute('data-ml'));
    if (isOz) {
      let ozVal = (val / 30).toFixed(2).replace(/\.00$/, '');
      el.innerText = ozVal + ' oz';
    } else {
      el.innerText = val + ' ml';
    }
  });
  
  document.getElementById('unitToggle').innerText = isOz ? "Přepnout na Ml" : "Přepnout na Oz";
}
</script>

---

# Drinky

---

## Bahama Mama
* **<span class="unit-ml" data-ml="30">30 ml</span>** tmavý rum (např. Plantation Original Dark)
* **<span class="unit-ml" data-ml="30">30 ml</span>** kokosový rum nebo vodka (např. Malibu, Espero, Finlandia)
* **<span class="unit-ml" data-ml="15">15 ml</span>** grenadina (případně třešňový sirup)
* **<span class="unit-ml" data-ml="60">60 ml</span>** čerstvá pomerančová šťáva
* **<span class="unit-ml" data-ml="60">60 ml</span>** čerstvá ananasová šťáva
* pár kapek šťávy z citronu nebo limetky

**Postup:** Vše vložíme do shakeru, pořádně protřepeme a nalijeme do sklenice s ledem.

---

## Dark ‘n Stormy
* **<span class="unit-ml" data-ml="60">60 ml</span>** tmavý rum (např. Gosling’s Black Seal, ideálně overproof)
* **<span class="unit-ml" data-ml="45">45 ml</span>** čerstvě vymačkaná limetková šťáva
* **cca <span class="unit-ml" data-ml="150">150 ml</span>** zázvorové pivo (případně ginger ale)

**Postup:** Šťávu smícháme s pivem, přidáme led a nahoru opatrně nalijeme (klidně přes lžičku) "mráček" rumu. Před konzumací rozmíchat.

---

## Tequila Sunrise
* **<span class="unit-ml" data-ml="60">60 ml</span>** blanco tequila (případně vodka pro Russian Sunrise)
* **<span class="unit-ml" data-ml="120">120 ml</span>** čerstvě vymačkaný pomerančový džus
* **<span class="unit-ml" data-ml="7">7 ml</span>** grenadina (případně třešňový sirup)

**Postup:** Přidejte tequilu a pak pomerančový džus do vychlazené sklenice naplněné ledem. Navrch nalijte grenadinu, která klesne na dno a vytvoří efekt vycházejícího slunce.

---

## Margarita
* **<span class="unit-ml" data-ml="60">60 ml</span>** blanco tequila
* **<span class="unit-ml" data-ml="15">15 ml</span>** pomerančový likér (Cointreau nebo Triple Sec)
* **<span class="unit-ml" data-ml="30">30 ml</span>** šťáva z čerstvé limetky
* **<span class="unit-ml" data-ml="15">15 ml</span>** agávový nebo simple sirup

**Postup:** Vše vložíme do shakeru, pořádně protřepeme a nalijeme do sklenice s ledem.

---

## Long Island Iced Tea
* **<span class="unit-ml" data-ml="15">15 ml</span>** vodka
* **<span class="unit-ml" data-ml="15">15 ml</span>** bílý rum
* **<span class="unit-ml" data-ml="15">15 ml</span>** tequila
* **<span class="unit-ml" data-ml="15">15 ml</span>** gin
* **<span class="unit-ml" data-ml="15">15 ml</span>** Cointreau nebo Triple Sec
* **<span class="unit-ml" data-ml="15">15 ml</span>** citronová šťáva
* **<span class="unit-ml" data-ml="15">15 ml</span>** cukrový sirup
* **<span class="unit-ml" data-ml="60">60 ml</span>** Coca-Cola

**Postup:** Vše (kromě Coly) vložíme do shakeru, protřepeme, nalijeme do sklenice s ledem a dolijeme Colou.

---

## Blue Hawaii
* **<span class="unit-ml" data-ml="25">25 ml</span>** vodka
* **<span class="unit-ml" data-ml="25">25 ml</span>** bílý rum
* **<span class="unit-ml" data-ml="15">15 ml</span>** likér Blue Curaçao
* **<span class="unit-ml" data-ml="20">20 ml</span>** šťáva z citronu nebo limetky
* **<span class="unit-ml" data-ml="10">10 ml</span>** simple sirup
* **<span class="unit-ml" data-ml="90">90 ml</span>** ananasová šťáva

**Postup:** Vše vložíme do shakeru, pořádně protřepeme a nalijeme do sklenice s ledem.

---

## Cuba Libre (preferovaná verze)
* **<span class="unit-ml" data-ml="30">30 ml</span>** bílý kubánský rum
* **<span class="unit-ml" data-ml="120">120 ml</span>** Royal Crown Cola, Coca-Cola
* pár kapek šťávy z citronu nebo limetky

**Postup:** Vše smíchat ve sklenici (**<span class="unit-ml" data-ml="200">200 ml</span>**) s ledem.

---

## Mojito
* **<span class="unit-ml" data-ml="40">40 ml</span>** bílý rum (overproofy fungují také dobře)
* **<span class="unit-ml" data-ml="30">30 ml</span>** limetková/citronová šťáva
* **8–12 ks** lístků máty (hrst)
* **2 ČL** třtinový cukr
* **<span class="unit-ml" data-ml="200">200 ml</span>** soda
* led (drcený nebo kostky)

**Postup:** Vložte mátu (trochu jí pomačkejte), rum, cukr a šťávu. Dobře promíchejte, dokud se cukr nerozpustí. Zasypte ledem a znovu pořádně promíchejte.

---

## Queen's Park Swizzle
* **8 ks** lístků máty
* **<span class="unit-ml" data-ml="60">60 ml</span>** bílý rum
* **<span class="unit-ml" data-ml="25">25 ml</span>** limetková šťáva
* **<span class="unit-ml" data-ml="15">15 ml</span>** simple sirup
* **2 dash** Angostura Bitters
* led (drcený nebo kostky)

**Postup:** Vložte mátu(trochu jí pomačkejte), rum, sirup a šťávu. Dobře promíchejte, zasypte ledem a znovu promíchejte.

---

## Piña Colada
* **<span class="unit-ml" data-ml="60">60 ml</span>** bílý rum
* **<span class="unit-ml" data-ml="30">30 ml</span>** kokosový krém, mléko, nebo **<span class="unit-ml" data-ml="15">15 ml</span>** sirupu + citrusy
* **<span class="unit-ml" data-ml="90">90 ml</span>** ananasová šťáva
* pár kapek citronové, nebo limetkové šťávy

**Postup (zjednodušený):** Vše v shakeru protřepat a nalít na led.
**Postup (normální):** Vše vymixovat v elektrickém mixéru s ledem do hladka.

---

## Sex on the Beach
* **<span class="unit-ml" data-ml="40">40 ml</span>** vodka (Finlandia, Smirnoff Red)
* **<span class="unit-ml" data-ml="20">20 ml</span>** broskvová vodka/likér (Bols Peach)
* **<span class="unit-ml" data-ml="60">60 ml</span>** pomerančový džus
* **<span class="unit-ml" data-ml="90">90 ml</span>** brusinkový džus (průměr z 60–120 ml)

**Postup:** V šejkru s ledem vyšejkrujeme vodky a pomerančový džus. Nalijeme do sklenice. Krouživým pohybem dolijeme brusinkový džus a lehce promíchneme pro barevný přechod.

---

## Daiquiri
* **<span class="unit-ml" data-ml="50">50 ml</span>** bílý rum
* **<span class="unit-ml" data-ml="20">20 ml</span>** limetková šťáva
* **<span class="unit-ml" data-ml="10">10 ml</span>** simple sirup

**Postup:** Vše vložíme do sklenice s ledem a promícháme (nebo v šejkru).

---

## Gimlet
* **<span class="unit-ml" data-ml="50">50 ml</span>** gin
* **<span class="unit-ml" data-ml="20">20 ml</span>** limetková šťáva
* *volitelně:* **<span class="unit-ml" data-ml="7">7 ml</span>** simple sirup

**Postup:** Vše vložíme do sklenice s ledem a promícháme.

---

## Old Fashioned
* **<span class="unit-ml" data-ml="60">60 ml</span>** whisky nebo bourbon
* **<span class="unit-ml" data-ml="8">8 ml</span>** simple sirup
* **2 dash** Angostura Bitters (nebo Tatratea bitters)

**Postup:** Smíchat ve sklenici s ledem (nebo v šejkru). Tradičně ozdobit a zastříknout pomerančovou kůrou.

---

## Manhattan
* **<span class="unit-ml" data-ml="50">50 ml</span>** Whiskey
* **<span class="unit-ml" data-ml="20">20 ml</span>** sladký červený vermut
* **1 dash** Angostura Bitters (či Tatratea bitters)

**Postup:** Vše smíchat ve sklenici s ledem.