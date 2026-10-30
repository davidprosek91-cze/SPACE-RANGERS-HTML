# Space Rangers – Havirov Coin Edition 🚀

**Verze 3.2 – Mercenary & Craft Update**
© 2026 David Prošek

Vesmírná arkádová hra v jediném HTML souboru. Kombinuje souboje, obchodování, těžbu asteroidů, crafting, RPG skilly, úkoly a simulovaný multiplayer. Inspirováno klasikou *Space Rangers*, *X3* a *Escape Velocity*.


---

## 🎮 O hře

Staňte se rangerem v rozlehlé galaxii plné planet, asteroidů, obchodních lodí a pirátů. Prozkoumávejte systémy, obchodujte, plňte úkoly, vylepšujte loď, těžte suroviny a vyrábějte zařízení pro svůj trup.

Hra běží přímo v prohlížeči – stačí otevřít `index.html`. Není potřeba instalace, server ani externí knihovny.

---

## ▶️ Rychlý start

1. Otevřete soubor `index.html` v moderním prohlížeči (Chrome, Firefox, Edge).
2. V menu zvolte **Nová hra** nebo **Načíst hru**.
3. Ovládejte loď pomocí `WASD` / šipek, střílejte mezerníkem a prozkoumávejte galaxii.

Hra se ukládá automaticky do prohlížeče (`localStorage`), takže po zavření stačí hru znovu načíst.

---

## ✨ Hlavní funkce

- **Plynulé ovládání lodi** – WASD/šipky, rotace, tah, brzdění, míření myší.
- **Obchodování** – dynamické ceny podle typu stanice a nabídky zboží.
- **Těžba asteroidů** – suroviny (Ruda, Zlato, Platina, Krystaly, Komponenty…).
- **Crafting** – 29 receptů na trvalá vylepšení lodi (trup, štíty, motor, zbraně, náklad, palivo, regenerace, radar, gyro).
- **Vylepšení lodi** – neomezené levely pro trup, štíty, rychlost, náklad a palivo.
- **Skill strom** – obchodování, štíty, zbraně, motor a náklad (max. 100).
- **Úkoly rangerů** – doručování, sběr surovin, likvidace pirátů za odměnu v HVC.
- **Automatický boj** – loď sama útočí na nejbližší cíl.
- **Najímání obchodních lodí** – ochrana v boji, prodej/nákup na dálku, palivo.
- **Simulovaný multiplayer** – ostatní hráči se pohybují v reálném čase.
- **Mapa galaxie** – teleport mezi planetami a přechod do dalších galaxií za kredity.
- **Ukládání** – automaticky každých ~15 sekund + ruční načtení z menu.

---

## 🕹 Ovládání

### Menu

| Klávesa | Akce |
|---|---|
| `1` | Nová hra |
| `2` | Načíst hru |
| `3` | Nápověda |
| `4` | Kredity |
| `5` | Multiplayer |

### Let a boj

| Klávesa | Akce |
|---|---|
| `W` / `↑` | Tah motoru vpřed |
| `S` / `↓` | Zpětný tah / brzdění |
| `A` / `D` / `←` / `→` | Rotace lodi |
| `Mezerník` / pravé tlačítko myši | Střelba |
| Levé tlačítko myši | Zamíření a zrychlení k cíli |
| `E` | Zapnout/vypnout automatický boj |
| `M` | Mapa galaxie |
| `ESC` | Zavřít obrazovku / návrat do menu |

### Ekonomika, stanice a těžba

| Klávesa | Akce |
|---|---|
| `T` | Komunikace s obchodní lodí (nákup / prodej / palivo / nájem) |
| `F` | Nákup paliva (u stanice) |
| `Q` | Úkoly (u stanice) |
| `U` | Vylepšení lodi (u stanice) |
| `P` | Skill strom (u stanice) |
| `C` | Crafting (u stanice); mimo stanici otevře kredity |
| `I` | Inventář (u stanice) |
| `K` | Start/stop těžby asteroidu |
| `L` | Historie a statistiky těžby |
| `J` | Sebrat předměty v dosahu |
| `B` | Zobrazit stav peněženky |

### Obrazovka obchodní lodi

| Klávesa | Akce |
|---|---|
| `1` | Nákup zboží |
| `2` | Prodej nákladu |
| `3` | Nákup paliva |
| `4` | Najmout loď pro boj |
| `5` | Propustit najatou loď |

### Obrazovka paliva

| Klávesa | Akce |
|---|---|
| `1` | 10 paliva (0,05 HVC) |
| `2` | 25 paliva (0,12 HVC) |
| `3` | 50 paliva (0,25 HVC) |
| `4` | 100 paliva (0,50 HVC) |

---

## 💰 Peněženka HVC

- Měna ve hře je **HVC (Havirov Coin)**.
- Peněženka se ukládá do `localStorage` pod klíčem `spaceRangersWallet`.
- Zůstatek peněženky se používá jako herní kredity.
- Adresa peněženky má formát `SR-XXXXXXXX`.
- Žádná kryptoměnová API ani externí peněženky se nepoužívají.

---

## 🪨 Těžba a crafting

1. Přibližte se k asteroidu a stiskněte `K`.
2. Loď těží suroviny, které se ukládají do nákladu.
3. V doku otevřete crafting (`C`).
4. Ze surovin vyrábíte trvalá vylepšení, která se automaticky nasadí do příslušného slotu.

Mezi suroviny patří například Ruda, Zlato, Stříbro, Platina, Krystaly, Křemík, Uhlí, Síra, Měď, Železo, Titan a Kobalt.

---

## 🗺 Galaxie

| # | Galaxie | Charakter |
|---|---|---|
| 0 | **Havirov** | Domovská galaxie – bezpečná zóna |
| 1 | **Nova Terra** | Průmyslová galaxie – hodně obchodu |
| 2 | **Crimson Belt** | Pirátská zóna – nebezpečí |
| 3 | **Emerald Expanse** | Vzácná galaxie – bohaté asteroidy |

Typy stanic: Planeta, Doky, Obchodní stanice, Hi-Tech Lab a Pirátský klub. Každá stanice má jiný sortiment a cenové násobiče.

---

## 💾 Ukládání

- **Pozice, loď, náklad, skilly, vylepšení a galaxie:** `localStorage` → `spaceRangersSave`.
- **Peněženka HVC:** `localStorage` → `spaceRangersWallet`.
- Automatické ukládání probíhá každých ~15 sekund během hry.
- Ruční načtení je dostupné v menu přes **Načíst hru**.

> Vymazáním dat pro danou stránku v prohlížeči smažete i svůj postup.

---

## 📦 Technické informace

- Čisté **HTML + CSS + JavaScript**, bez externích knihoven a bez serveru.
- Vše je obsaženo v jediném souboru `index.html`.
- Vykreslování přes `<canvas>` (1024 × 768, responzivní škálování).
- Uložení ve formátu JSON v `localStorage`.
- Všechny texty jsou v češtině.

### Struktura projektu

```
SPACE-RANGERS-HTML-main/
├── index.html   # celá hra (HTML, CSS, JavaScript)
├── README.md    # původní dokumentace
└── read.me      # tato aktuální dokumentace
```

---

## 🙏 Poděkování

- Původní hra: **Elemental Games** – *Space Rangers* (2002)
- Inspirace: *Space Rangers*, *X3*, *Escape Velocity*
- Autor: **David Prošek**
- ❤️ Powered by Karma – EverythingIsLife

---

## 📜 Licence

© 2026 David Prošek. Všechna práva vyhrazena.
