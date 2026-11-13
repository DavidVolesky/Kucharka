---
layout: default
title: Párky
parent: Uzeniny
---

# Párky

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

### Obecné zásady výroby párků

- **Textura:** Párky vyžadují velmi jemnou **spojku** (dílo musí být dokonale vykutrované na jemnou pastu).
- **Teplota:** Při kutrování je kritické udržet teplotu pod **12 °C** (používejte ledovou tříšť nebo velmi studenou
  vodu).
- **Plnění:** Párky se standardně plní do tenkých **skopových střev**.
- **Finální úprava:** Po vytažení z udírny (nebo po ovaření) je nutné párky okamžitě **prudce zachladit** v ledové vodní
  lázni. Tím dojde k vypnutí střívka a párky budou při skusu krásně **křupat**.

---

### Vídeňské párky

*Jemné párky z čistě vepřového masa (nebo s malým podílem hovězí spojky).*

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli (Praganda)
- <span class="val-calc" data-base="3">3</span> g barevného pepře
- <span class="val-calc" data-base="1">1</span> g muškátového oříšku
- <span class="val-calc" data-base="2">2</span> g sladké papriky
- <span class="val-calc" data-base="0.5">0.5</span> g koriandru
- <span class="val-calc" data-base="0.5">0.5</span> g zázvoru
- <span class="val-calc" data-base="150">150</span> ml ledové vody
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva

---

### Debrecínské párky

*Charakteristické hrubší vložkou z bůčku.*

**Složení:** Mix vepřového a hovězího masa. Jako vložka se používá vepřový bok mletý na 8 mm, zbytek je jemná spojka.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli
- <span class="val-calc" data-base="3">3</span> g sladké papriky
- <span class="val-calc" data-base="3">3</span> g barevného pepře
- <span class="val-calc" data-base="1">1</span> g mletého kmínu
- <span class="val-calc" data-base="1">1</span> g granulovaného česneku
- <span class="val-calc" data-base="0.5">0.5</span> g zázvoru
- <span class="val-calc" data-base="150">150</span> ml ledové vody
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva

---

### Spišské párky

*Tradiční párky s výrazným podílem papriky.*

**Složení:** Mix vepřového a hovězího masa, kutrované na velmi jemnou konzistenci.

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="16">16</span> g řeznické soli
- <span class="val-calc" data-base="7">7</span> g sladké papriky
- <span class="val-calc" data-base="7">7</span> g pálivé papriky
- <span class="val-calc" data-base="100">100</span> ml ledové vody
- <span class="val-calc" data-base="0.5">0.5</span> sáčku prášku do pečiva