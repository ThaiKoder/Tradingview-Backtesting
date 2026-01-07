Voici un **README clair et structuré**, d’abord en **anglais**, puis en **français**, adapté exactement à ton script Pine Script.

Tu peux le copier tel quel dans un `README.md`.

---

# 📘 README (EN)

## RSI / RSI2 / Stochastic RSI Strategy Tester

### Overview

This TradingView **Pine Script v5 strategy** is a modular strategy tester based on:

* **RSI 1**
* **RSI 2**
* **Stochastic RSI**

Each indicator can be **enabled or disabled independently** using checkboxes.
The strategy automatically adapts its entry logic based on the active indicators.

---

## 🔧 Features

* ✅ Two independent RSI indicators (RSI 1 & RSI 2)
* ✅ Optional Stochastic RSI confirmation
* ✅ Checkbox-based logic (use only selected indicators)
* ✅ Automatic handling of all indicator combinations
* ✅ Long & Short entries
* ✅ Stop Loss & Take Profit defined in **ticks**
* ✅ Compatible with futures (NQ, ES, MNQ, MYM), crypto, and forex

---

## 📊 Indicators Logic

### RSI 1

* Configurable length
* Overbought / Oversold levels
* Long entry: RSI crosses **above** Overbought level
* Short entry: RSI crosses **below** Overbought level

### RSI 2

* Independent RSI with its own parameters
* Same crossover / crossunder logic as RSI 1

### Stochastic RSI

* Based on RSI 1
* Uses K/D crossovers
* Optional confirmation filter

---

## 🧠 Entry Logic

The strategy evaluates **only the indicators that are enabled**.

Examples:

* 1 only → entries based solely
* 2 only → both conditions must be valid
* all → all three must align
* If no indicator is enabled → **no trade**

All possible combinations are handled explicitly to ensure precise backtesting behavior.

---

## ⏱️ Risk Management (Ticks-based)

* Stop Loss and Take Profit are defined in **ticks**
* Automatically converted using `syminfo.mintick`
* SL/TP is placed relative to the **actual entry price**

This makes the strategy robust across different instruments.

---

## 📈 Visualization

* RSI 1 and RSI 2 plotted when enabled
* Stochastic RSI K & D plotted when enabled
* Reference horizontal levels at 70 and 30

---

## ⚠️ Notes

* This strategy is intended for **backtesting and research**
* Not financial advice
* Always validate results across multiple timeframes and instruments

---

---

# 📘 README (FR)

## RSI / RSI2 / Stochastic RSI – Strategy Tester

### Présentation

Cette **stratégie Pine Script v5 pour TradingView** est un strategy tester modulaire basé sur :

* **RSI 1**
* **RSI 2**
* **Stochastic RSI**

Chaque indicateur peut être **activé ou désactivé indépendamment** via des cases à cocher.
La logique d’entrée s’adapte automatiquement aux indicateurs sélectionnés.

---

## 🔧 Fonctionnalités

* ✅ Deux RSI indépendants (RSI 1 & RSI 2)
* ✅ Stochastic RSI optionnel
* ✅ Logique basée sur des checkboxes
* ✅ Gestion explicite de toutes les combinaisons
* ✅ Entrées Long et Short
* ✅ Stop Loss & Take Profit en **ticks**
* ✅ Compatible futures (NQ, ES, MNQ, MYM), crypto et forex

---

## 📊 Logique des indicateurs

### RSI 1

* Période configurable
* Niveaux Overbought / Oversold
* Entrée Long : croisement **au-dessus** du niveau Overbought
* Entrée Short : croisement **en dessous** du niveau Overbought

### RSI 2

* RSI secondaire totalement indépendant
* Même logique de croisement que RSI 1

### Stochastic RSI

* Calculé à partir du RSI 1
* Croisement K/D
* Sert de filtre de confirmation optionnel

---

## 🧠 Logique d’entrée

La stratégie **ne prend en compte que les indicateurs activés**.

Exemples :

* 1 seulement → une conditions doit être valides
* 2 seulement → deux conditions doivent être valides
* tout → les trois doivent être alignés
* Aucun indicateur actif → **aucune entrée**

Toutes les combinaisons sont gérées explicitement pour garantir un backtest fiable.

---

## ⏱️ Gestion du risque (en ticks)

* Stop Loss et Take Profit définis en **ticks**
* Conversion automatique via `syminfo.mintick`
* SL/TP placés par rapport au **prix réel d’entrée**

Cela garantit une cohérence parfaite sur tous les marchés.

---

## 📈 Visualisation

* RSI 1 et RSI 2 affichés uniquement s’ils sont activés
* Stochastic RSI K & D affichés si activés
* Lignes horizontales de référence à 70 et 30

---

## ⚠️ Remarques

* Stratégie destinée au **backtest et à la recherche**
* Ne constitue pas un conseil financier
* Toujours tester sur plusieurs marchés et timeframes

