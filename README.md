# 🛠️ Engineering Tools Hub

Webová platforma s profesionálnymi nástrojmi pre inžinierov, vývojárov elektroniky a technikov. Všetky nástroje sú optimalizované pre desktop aj mobilné zariadenia a bežia priamo v prehliadači bez potreby inštalácie.

## 🚀 Prehľad nástrojov

### 1. 🎨 Resistor Color Code & SMD Decoder
Komplexný dekodér pre rezistory.
* **Leaded:** Podpora pre 4-pásikové a 5-pásikové rezistory s vizualizáciou farby tela.
* **SMD:** Dekódovanie štandardných 3/4 ciferných kódov, R-zápisu (napr. 4R7) a precíznych kódov **EIA-96 (1%)**.

### 2. 🌀 SMD Reel Counter (SMD Reel Calculator)
Špecializovaný nástroj na odhad počtu komponentov na kotúči.
* **Matematický model:** Výpočet založený na dĺžke Archimedovej špirály pomocou numerickej integrácie (Simpsonovo pravidlo).
* **Korekčné faktory:** Implementácia korekcie na základe reálnych meraní (kompenzácia vôle pri navíjaní).
* **Vizualizácia:** Dynamické kreslenie špirály a meracích bodov na HTML5 Canvas.
* **Predvoľby:** Prednastavené hodnoty pre najpoužívanejšie typy pások (0.95T, 1.35T atď.).

### 3. ⚡ Ohm's Law Calculator
Rýchly výpočet základných elektrických veličín.
* Automatický výpočet zostávajúcich parametrov po zadaní dvoch známych hodnôt ($U, I, R, P$).

### 4. 🔋 Voltage Divider
Nástroj na návrh odporových deličov napätia.
* Výpočet výstupného napätia ($V_{out}$) v reálnom čase.
* Grafická schéma pre lepšiu orientáciu v zapojení.

### 5. 🏗️ basicMOST (WIP)
* Nástroj pre prácu s dátami a výrobnými vrstvami.

---

## 🛠️ Použité technológie

* **HTML5 & CSS3:** Moderná sémantika a štýlovanie.
* **Tailwind CSS:** Responzívny dizajn (Mobile-first prístup).
* **JavaScript (ES6+):** Logika výpočtov, numerická integrácia a manipulácia s DOM.
* **HTML5 Canvas API:** Pre vykresľovanie grafických modelov (SMD Reel).
* **GitHub Pages:** Hosting a kontinuálne nasadenie.

---

## 📈 Technické detaily (SMD Reel)

Výpočet dĺžky pásky $L$ nie je lineárny. Aplikácia rieši integrál:
$$L = \int_{0}^{\theta_{max}} \sqrt{(r_i + b\theta)^2 + b^2} d\theta$$
kde:
* $r_i$ je vnútorný polomer,
* $b$ je koeficient rastu špirály ($t / 2\pi$),
* $\theta$ je uhol natočenia.

Kvôli presnosti je tento integrál v aplikácii riešený numericky, čo zabezpečuje vysokú presnosť odhadu v porovnaní s jednoduchými matematickými aproximáciami.

---

## 📱 Inštalácia a spustenie

Nie je potrebná žiadna inštalácia. Stačí navštíviť:
`https://cuperpet.github.io/ingineering-tools/`