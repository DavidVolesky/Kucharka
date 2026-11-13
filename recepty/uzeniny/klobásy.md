---
layout: default
title: Klobásy
parent: Uzeniny
---

# Klobásy

<div style="background: #f4f4f4; padding: 15px; border: 1px solid #ddd; border-radius: 8px; margin-bottom: 20px;">
  <label for="meatInput" style="font-weight: bold; margin-right: 10px;">Zadej váhu masa (kg):</label>
  <input type="number" id="meatInput" value="1" step="0.5" min="0.1" oninput="calculateSausages()" style="padding: 8px; width: 100px; border: 1px solid #ccc; border-radius: 4px; font-size: 16px;">
  <span style="font-size: 0.9em; color: #666; margin-left: 10px;">(Recepty se automaticky přepočítají na zvolenou váhu)</span>
</div>

<script>
function calculateSausages() {
  const inputEl = document.getElementById('meatInput');
  let inputVal = parseFloat(inputEl.value);
  if (isNaN(inputVal) || inputVal < 0) { inputVal = 0; }
  
  document.querySelectorAll('.val-meat').forEach(el => {
    el.innerText = inputVal;
  });

  document.querySelectorAll('.val-calc').forEach(el => {
    let base = parseFloat(el.getAttribute('data-base'));
    let newVal = base * inputVal;
    
    if (base < 5) {
       el.innerText = parseFloat(newVal.toFixed(1));
    } else {
       el.innerText = Math.round(newVal);
    }
  });
}
document.addEventListener('DOMContentLoaded', calculateSausages);
</script>

---

### Obecné zásady výroby

- **Hygiena a trvanlivost:** Při výrobě většího množství používejte **granulovaný česnek** (čerstvý česnek může způsobit
  dřívější kysnutí nebo kažení díla).
- **Teplota:** Teplota díla (masa) nesmí při míchání překročit **12 °C**, aby se nerozpustil tuk a klobása nebyla tzv.
  *"podlitá"* (tuk vyteče pod střívko).
- **Složení:**
    - **Spojka:** Jemně namleté (ideálně kutrované) maso s vodou, které drží klobásu pohromadě.
    - **Vložka:** Hrubě mleté nebo krájené maso na kostičky, které vytváří mozaiku a texturu.
- **Aditiva:**
    - **Voda:** Zvyšuje vaznost (bez ní jsou klobásy po uvaření/uzení drobivé).
    - **Cukr:** Podporuje karamelizaci pro lepší barvu při grilování.
    - **Dextróza:** Podporuje mléčné kvašení u fermentovaných výrobků a stabilitu barvy.
    - **Prášek do pečiva:** Obsahuje fosfáty a škrob, které pomáhají udržet šťávu a pevnost.
        - *Dávkování:* Půl balíčku na 1 kg masa pro výrobky, které se dále tepelně opracovávají.
        - *Výhoda:* Pomáhá posunout kritickou hranici teploty při míchání, pokud není možné udržet dílo pod 12 °C (např.
          v letních podmínkách).

---

## 1. Klasické klobásy

### Ostravská klobása

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli (Pragandy)
- <span class="val-calc" data-base="5">5</span> g cukru
- <span class="val-calc" data-base="7">7</span> g barevného pepře
- <span class="val-calc" data-base="3">3</span> g mletého kmínu
- <span class="val-calc" data-base="8">8</span> g granulovaného česneku
- <span class="val-calc" data-base="100">100</span> ml vody

---

### Valašská klobása

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli
- <span class="val-calc" data-base="2">2</span> g cukru
- <span class="val-calc" data-base="7">7</span> g barevného pepře
- <span class="val-calc" data-base="3">3</span> g mletého kmínu
- <span class="val-calc" data-base="8">8</span> g granulovaného česneku
- <span class="val-calc" data-base="2">2</span> g majoránky
- <span class="val-calc" data-base="0.5">0.5</span> g nového koření
- <span class="val-calc" data-base="0.5">0.5</span> g mletého koriandru
- <span class="val-calc" data-base="100">100</span> ml vody

---

### Špekáčky

**Příprava:** Jemná spojka a hrubá vložka (**hřbetní sádlo**) v poměru **2:1**. Udit, poté ovařit a prudce zachladit.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli
- <span class="val-calc" data-base="2">2</span> g cukru
- <span class="val-calc" data-base="5">5</span> g barevného pepře
- <span class="val-calc" data-base="1.5">1.5</span> g muškátového oříšku (nebo mix s květem)
- <span class="val-calc" data-base="5">5</span> g sladké papriky
- <span class="val-calc" data-base="4">4</span> g granulovaného česneku
- <span class="val-calc" data-base="150">150</span> ml vody

---

### Käsekrainer (Sýrová klobása)

**Složení masa:** 1 díl hovězí přední, 1 díl bůček, 2 díly krkovice/plec/kýta.  
**Příprava:** Jemná spojka + vložka ze sýra.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="14">14</span> g řeznické soli
- <span class="val-calc" data-base="2">2</span> g cukru
- <span class="val-calc" data-base="200">200</span> g sýra (Gouda, Čedar, Ementál) – nakrájený na kostičky
- <span class="val-calc" data-base="1.5">1.5</span> g muškátového oříšku
- <span class="val-calc" data-base="1.5">1.5</span> g koriandru
- <span class="val-calc" data-base="1.5">1.5</span> g zázvoru
- <span class="val-calc" data-base="5">5</span> g granulovaného česneku
- <span class="val-calc" data-base="50">50</span> ml vody
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva

---

### Klobásy s medvědím česnekem

**Složení masa:** 1 díl vepřový bůček, 3 díly libové hovězí/vepřové. Lze grilovat, udit i vařit.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli
- <span class="val-calc" data-base="2">2</span> g cukru
- <span class="val-calc" data-base="2">2</span> g mletého kmínu
- <span class="val-calc" data-base="2">2</span> g barevného pepře
- <span class="val-calc" data-base="2">2</span> g sladké papriky
- <span class="val-calc" data-base="0.5">0.5</span> g zázvoru
- <span class="val-calc" data-base="40">40</span>+ g medvědího česneku
- <span class="val-calc" data-base="150">150</span> ml vody

---

## 2. Fermentované klobásy

### Čabajka

**Příprava:** Maso na hrubo (poměr kýta/plec ku boku 4:3 nebo 4:1). Po naražení nechat **3 dny fermentovat** při
pokojové teplotě. Následně udit **24 hodin studeným kouřem** a nechat **měsíc zrát** (vysychat).

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="19">19</span> g řeznické soli
- <span class="val-calc" data-base="5">5</span> g dextrózy
- <span class="val-calc" data-base="10">10</span> g sladké papriky
- <span class="val-calc" data-base="10">10</span> g pálivé papriky
- <span class="val-calc" data-base="5">5</span> g barevného pepře
- <span class="val-calc" data-base="2">2</span> g mletého kmínu
- <span class="val-calc" data-base="4">4</span> g granulovaného česneku
- <span class="val-calc" data-base="0.5">0.5</span> g nového koření
- <span class="val-calc" data-base="1">1</span> g zázvoru
- *(volitelně: <span class="val-calc" data-base="1">1</span> g muškátového oříšku)*

---

### Chorizo

**Příprava:** Bůček a plec (1:1), mletí na 8 mm. Nechat **2 dny fermentovat** při pokojové teplotě a pak nechat **měsíc
vysychat** v chladu.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="19">19</span> g řeznické soli
- <span class="val-calc" data-base="2">2</span> g sušeného oregana
- <span class="val-calc" data-base="10">10</span> g sladké uzené papriky
- <span class="val-calc" data-base="10">10</span> g pálivé uzené papriky
- <span class="val-calc" data-base="4">4</span> g pepře
- <span class="val-calc" data-base="4">4</span> g granulovaného česneku
- <span class="val-calc" data-base="3">3</span> g dextrózy

---

## 3. Klobásy pro okamžitou spotřebu

### Salsiccia

**Příprava:** Pouze libové vepřové, mletí nahrubo. Plnit do tenkých vepřových střev. Určeno k okamžitému grilování.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g obyčejné soli (nikoliv řeznické)
- <span class="val-calc" data-base="2">2</span> g cukru
- <span class="val-calc" data-base="100">100</span> g parmazánu
- 5 stroužků česneku
- 20 lístků šalvěje (bez stonků)
- <span class="val-calc" data-base="150">150</span> ml suchého bílého vína
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva

---

### Vinná klobása

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="14">14</span> g soli
- <span class="val-calc" data-base="120">120</span> g žemle (namočené v tekutině)
- **Tekutina:** (<span class="val-calc" data-base="90">90</span> ml bílého
  vína + <span class="val-calc" data-base="100">100</span> ml vody + <span class="val-calc" data-base="40">40</span> ml
  smetany) NEBO (<span class="val-calc" data-base="90">90</span> ml vína + <span class="val-calc" data-base="140">
  140</span> ml mléka)
- **Koření:** 3 g hotové směsi NEBO (<span class="val-calc" data-base="1">1</span> g bílý
  pepř, <span class="val-calc" data-base="1">1</span> g muškátový oříšek, <span class="val-calc" data-base="0.5">
  0.5</span> g citronová kůra a <span class="val-calc" data-base="0.5">0.5</span> g mletý hřebíček)

---

## 4. Bratwürste (Grilovací klobásy)

**Tepelná úprava (Sous-vide):** Vložit do lázně o teplotě **80 °C**. Jakmile vnitřní teplota klobásy dosáhne **71 °C**,
dojde k bezpečné pasterizaci.

### Norimberská klobása (Nürnberger Rostbratwurst)

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g soli
- <span class="val-calc" data-base="1">1</span> g cukru
- <span class="val-calc" data-base="4">4</span> g majoránky
- <span class="val-calc" data-base="4">4</span> g barevného pepře
- <span class="val-calc" data-base="0.5">0.5</span> g muškátového oříšku
- <span class="val-calc" data-base="0.5">0.5</span> g nového koření
- <span class="val-calc" data-base="100">100</span> ml vody
- <span class="val-calc" data-base="0.5">0.5</span> prášku do pečiva

---

### Mnichovská bílá klobása (Munich Weisswurst)

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g soli
- <span class="val-calc" data-base="1">1</span> g cukru
- <span class="val-calc" data-base="4">4</span> g barevného pepře
- <span class="val-calc" data-base="0.5">0.5</span> g muškátového oříšku
- <span class="val-calc" data-base="1">1</span> g drceného hořčičného semínka
- <span class="val-calc" data-base="1">1</span> g citronové kůry (sušené nebo z 1 čerstvého citronu)
- <span class="val-calc" data-base="15">15</span> g čerstvé petržele (nebo 5 g sušené)
- <span class="val-calc" data-base="100">100</span> ml vody
- <span class="val-calc" data-base="0.5">0.5</span> prášku do pečiva

---

### Bavorská klobása (Bayerische Bratwurst)

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g soli
- <span class="val-calc" data-base="1">1</span> g cukru
- <span class="val-calc" data-base="4">4</span> g barevného pepře
- <span class="val-calc" data-base="0.5">0.5</span> g nového koření
- <span class="val-calc" data-base="2">2</span> g majoránky
- <span class="val-calc" data-base="0.5">0.5</span> g muškátového oříšku
- <span class="val-calc" data-base="0.5">0.5</span> g mletého koriandru
- <span class="val-calc" data-base="100">100</span> ml vody
- <span class="val-calc" data-base="0.5">0.5</span> prášku do pečiva

---

### Moje klobása (Meine Bratwurst)

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g soli
- <span class="val-calc" data-base="1">1</span> g cukru
- <span class="val-calc" data-base="2">2</span> g majoránky
- <span class="val-calc" data-base="5">5</span> g barevného pepře
- <span class="val-calc" data-base="0.5">0.5</span> g muškátového oříšku
- <span class="val-calc" data-base="0.5">0.5</span> g muškátového květu (nebo navýšit oříšek na 1 g celkem)
- <span class="val-calc" data-base="0.5">0.5</span> g nového koření
- <span class="val-calc" data-base="0.5">0.5</span> g mletého kmínu
- <span class="val-calc" data-base="0.5">0.5</span> g mletého zázvoru
- <span class="val-calc" data-base="0.5">0.5</span> g mletého koriandru
- <span class="val-calc" data-base="100">100</span> ml vody
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva
- *(volitelně: <span class="val-calc" data-base="0.5">0.5</span>–<span class="val-calc" data-base="2">2</span> g
  drceného hořčičného semínka)*