---
layout: default
title: Salámy
parent: Uzeniny
---

# Salámy

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

### Obecné zásady pro trvanlivé salámy

- **Zrání:** U fermentovaných salámů je klíčové dodržet teplotu a vlhkost při zrání, aby nedošlo k "uzavření" povrchu
  (příliš rychlému vyschnutí kraje), což by zastavilo vysychání středu.
- **Fermentace:** Dextróza slouží jako potrava pro bakterie mléčného kvašení, které zajistí typickou navinulou chuť a
  bezpečnost výrobku.

---

## 1. Fermentované a trvanlivé salámy

### Lovecký salám (Lovečák)

**Složení masa:** 2 díly vepřová plec, 2 díly vepřový bůček, 1 díl hovězí přední.  
**Příprava:** Po naražení do hranatých forem (nebo klasických střev) nechat **2–3 dny fermentovat** při pokojové
teplotě. Poté udit **studeným kouřem po dobu 24 hodin**. Následně nechat v chladu a mírném průvanu vysychat (zrání trvá
dle průměru střeva několik týdnů).

*Koření na <span class="val-meat">1</span> kg masa:*

- <span class="val-calc" data-base="17">17</span> g řeznické soli (Praganda)
- <span class="val-calc" data-base="3">3</span> g dextrózy
- <span class="val-calc" data-base="3">3</span> g pepře
- <span class="val-calc" data-base="2">2</span> g mletého kmínu
- <span class="val-calc" data-base="0.5">0.5</span> g mletého hřebíčku
- <span class="val-calc" data-base="4">4</span> g granulovaného česneku