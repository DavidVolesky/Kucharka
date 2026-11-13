---
layout: default
title: Šunky a uzené boky
parent: Uzeniny
---

# Šunky a uzené boky

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

### Obecné zásady pro uzení a sušení

- **Proležení:** U suchého nasolování se maso důkladně potře směsí a nechá v chladu (cca 4 °C) odpočívat. U sušených
  šunek se doba proležení odvíjí od výšky masa (standardně cca 1–2 týdny).
- **Praganda:** Řeznická sůl zajišťuje typickou růžovou barvu a chrání maso před kažením během sušení.
- **Sušení:** Probíhá v temné místnosti s mírným prouděním vzduchu při teplotě kolem 12–15 °C.

---

## 1. Sušené a studeným kouřem uzené

### Schwarzwaldská šunka

*Ideální z vepřové kýty (ořech nebo šál), lze použít i vepřový bok.*

**Postup:** Maso důkladně nasolit a okořenit, nechat proležet v chladu. Poté udit **24 hodin studeným kouřem** a
následně nechat **3 týdny sušit** (zrání).

*Suroviny a koření (na <span class="val-meat">1</span> kg masa):*

- <span class="val-calc" data-base="28">28</span> g řeznické soli – pro sušené výrobky je dávka vyšší
- Jalovec
- Koriandr
- Pepř

---

### Slovenský bok

*Tradiční sušený bůček s čistou chutí masa a kouře. Stejným způsobem lze udělat i hřbetní sádlo, coby špek na vaření.*

**Postup:** Bok nasolit Pragandou, nechat proležet. Udit **24 hodin studeným kouřem** a poté nechat **2 týdny sušit**
(dozrát).

*Suroviny (na <span class="val-meat">1</span> kg masa):*

- <span class="val-calc" data-base="25">25</span> g řeznické soli

---

## 2. Uzené teplým kouřem

### Tátův bok

*Klasický uzený bůček pro přímou konzumaci nebo vaření.*

**Postup:** Maso nasolit Pragandou, nechat proležet v lednici (u teplého uzení ideálně 1–2 týdny dle velikosti).
Následně předvařit v sous-vide lázni. Poté **vyudit teplým kouřem** (cca 70–80 °C) dozlatova.

*Suroviny (na <span class="val-meat">1</span> kg masa):*

- <span class="val-calc" data-base="22">22</span> g řeznické soli *(standardní dávka pro uzení teplým kouřem)*