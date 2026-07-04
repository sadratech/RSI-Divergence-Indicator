# RSI Divergence Indicator

> 🇬🇧 English · 🇫🇷 Français

An RSI divergence indicator for TradingView, written in Pine Script v5.
It detects divergence between **price** and the **RSI** oscillator.

Un indicateur de divergence RSI pour TradingView, écrit en Pine Script v5.
Il détecte la divergence entre le **prix** et l'oscillateur **RSI**.

---

## 🇬🇧 English

### What it does

The indicator compares price pivots with RSI pivots to spot two types of regular divergence:

- 🟢 **Bullish divergence** — price makes a *lower low* while RSI makes a *higher low* → potential upward reversal. Marked with a green `Bull` label below the candle.
- 🔴 **Bearish divergence** — price makes a *higher high* while RSI makes a *lower high* → potential downward reversal. Marked with a red `Bear` label above the candle.

### Installation

1. Open the **Pine Editor** in TradingView.
2. Copy and paste the contents of [`RSI_Divergence.pine`](RSI_Divergence.pine).
3. Click **Add to chart**.

### Settings

| Input | Default | Description |
|---|---|---|
| RSI period | 14 | Length of the RSI calculation |
| Pivot Left / Right | 5 / 5 | Sensitivity for detecting highs and lows |
| Min / Max range | 5 / 60 | Allowed distance (in bars) between two pivots |
| Show Bullish / Bearish | on | Toggle each divergence type |

### Alerts

Two alert conditions are built in: **RSI Bullish Divergence** and **RSI Bearish Divergence**. Add them from TradingView's alert menu.

### Note

Because of the right pivot lookback (`Pivot Right`), labels are confirmed a few bars after they form. This delay is inherent to every divergence indicator and prevents false signals.

---

## 🇫🇷 Français

### Ce qu'il fait

L'indicateur compare les pivots du prix avec les pivots du RSI pour repérer deux types de divergence classique :

- 🟢 **Divergence haussière** — le prix forme un *creux plus bas* tandis que le RSI forme un *creux plus haut* → possible retournement à la hausse. Signalée par une étiquette verte `Bull` sous la bougie.
- 🔴 **Divergence baissière** — le prix forme un *sommet plus haut* tandis que le RSI forme un *sommet plus bas* → possible retournement à la baisse. Signalée par une étiquette rouge `Bear` au-dessus de la bougie.

### Installation

1. Ouvrez le **Pine Editor** dans TradingView.
2. Copiez et collez le contenu de [`RSI_Divergence.pine`](RSI_Divergence.pine).
3. Cliquez sur **Add to chart** (Ajouter au graphique).

### Paramètres

| Entrée | Défaut | Description |
|---|---|---|
| Période RSI | 14 | Longueur du calcul du RSI |
| Pivot gauche / droit | 5 / 5 | Sensibilité de détection des sommets et creux |
| Distance min / max | 5 / 60 | Distance autorisée (en bougies) entre deux pivots |
| Afficher haussière / baissière | activé | Active ou désactive chaque type de divergence |

### Alertes

Deux conditions d'alerte sont intégrées : **RSI Bullish Divergence** (divergence haussière) et **RSI Bearish Divergence** (divergence baissière). Ajoutez-les depuis le menu d'alertes de TradingView.

### Remarque

En raison du décalage du pivot droit (`Pivot Right`), les étiquettes sont confirmées quelques bougies après leur formation. Ce délai est propre à tout indicateur de divergence et évite les faux signaux.

---

## License / Licence

MIT
