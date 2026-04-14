# 📜 La Gazette du Trône

> *« Tempus stercoris pecunia est. »*
>
> — Proverbe apocryphe, attribué à un consultant stoïcien du II<sup>e</sup> siècle

**La Gazette du Trône** est un bulletin officiel, éphémère et chiffré, qui calcule le **préjudice économique** occasionné par chacune de vos pauses-sanitaires sur le temps facturé. L'Observatoire National du Préjudice Défécatoire — fondé en **MCMLXVII** — publie ses conclusions en deux éditions : matinale et nocturne.

---

## 🎯 Fonctionnalité principale

Vous déclarez votre TJ, vos heures ouvrées, la durée moyenne d'évacuation, le trajet aller vers le cabinet et la fréquence quotidienne. La Gazette en déduit instantanément le préjudice par séance, selon :

```
Préjudice = TJ ÷ (H × 60) × [ m_💩 + 2 × s_🚶 ÷ 60 ]

 où    TJ    = taux journalier (€)
       H     = heures facturables / jour
       m_💩  = durée d'évacuation (minutes)
       s_🚶  = trajet aller-simple (secondes)
```

Le trajet est comptabilisé **aller ET retour** d'office. L'Observatoire ne saurait tolérer la moindre approximation.

---

## ✨ Ce que publie la Gazette

| § | Rubrique | Contenu |
|---|----------|---------|
| I | **Bulletin principal** | Le préjudice unitaire par séance, classé sur une échelle officielle (*Anodin* → *Crise nationale*). |
| II | **Indicateurs macro-intestinaux** | Extrapolations journalière, mensuelle (22j), annuelle (220j), temps perdu, équivalent cafés, part de la journée ouvrée. |
| III | **Chronomètre officiel** | Cadran analogique pour mesurer une séance en direct, puis la consigner d'un geste. |
| IV | **Journal des séances** | Registre des dix dernières entrées, exportable en `.csv` (l'édition imprimée). |

Et, en marge : **ruban de cours** (« CAC-PQ 40 », « Indice du vélin », « Papier-toilette 12 rlx »), **tampon « confidentiel »** rotatif, **devise latine**, **cul-de-lampes** ❦, **œuf de Pâques** (cliquez cinq fois sur le titre).

---

## 🚀 Lancer la Gazette

Aucune dépendance. Aucun `npm install`. Aucun `build`.

```bash
# Option 1 — ouvrir directement
open index.html

# Option 2 — servir localement (toute alternative fait l'affaire)
python3 -m http.server 8000
# → http://localhost:8000
```

L'historique et la préférence d'édition (matin/soir) sont persistés dans le `localStorage` — rien ne quitte votre machine.

---

## 🎨 Direction artistique

| Aspect | Choix |
|--------|-------|
| **Concept** | Gazette ministérielle du XIX<sup>e</sup>, ton sérieusement absurde |
| **Typographie de titre** | [Fraunces](https://fonts.google.com/specimen/Fraunces) — variable, axes `opsz` 144, `wght` 900, `SOFT` 0 |
| **Typographie courante** | Fraunces à `opsz` plus petite, italiques `SOFT` élevée |
| **Chiffres & indicateurs** | [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono), `tabular-nums` |
| **Palette matinale** | Vélin `#F3E9D2`, encre `#14161C`, rouge signal `#A22525`, or `#9A7324` |
| **Palette nocturne** | Vélin brûlé `#161310`, encre claire `#EADEC1`, rouge adouci `#DE5656` |
| **Détails** | Grain de papier (SVG turbulence), culs-de-lampes, filet double, vignette périphérique |

---

## 🧪 Testé

Testé manuellement dans Chrome, en éditions **du matin** et **du soir**, en viewports **1400×1000** et **390×844**. Calcul validé à la main :

> TJ 600 € · 7,5 h · 6 min · 30 s · 2,5/j → **9,33 € / séance**, **23,33 € / jour**, **5 133 € / an** 💀

---

## 📐 Stack

Un seul fichier, `index.html`. HTML sémantique, CSS moderne (variables, `grid`, `clamp`, `font-variation-settings`), JavaScript vanilla. Aucun framework, aucun bundler, aucun tracker. Écrit pour durer.

---

## 🙏 Colophon

Publié sous l'égide de l'*Observatoire National du Préjudice Défécatoire*.
Rédacteur en chef : *un algorithme jovial*. Maquette et typographie : **Fraunces** & **JetBrains&nbsp;Mono**. Imprimé sur vélin numérique, en deux éditions — matinale & nocturne.

> § Fin de l'édition · Repli au cabinet autorisé §
