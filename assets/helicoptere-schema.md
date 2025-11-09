# Schéma Robinson R22 - Vue d'ensemble

## Vue Latérale Robinson R22

```
ROBINSON R22 - VUE LATÉRALE
═════════════════════════════

                ROTOR PRINCIPAL
            ┌─────────────────────┐
            │   PALE 1   PALE 2   │ ← Diamètre 7.67m
            └─────────────────────┘

     ROTOR DE QUEUE
   ┌─────────────────┐
   │   PALE 1   PALE 2│ ← Diamètre 1.42m
   └─────────────────┘

┌─────────────────────────────────────────────────┐
│              FUSELAGE PRINCIPAL                 │
├─────────────────────────────────────────────────┤
│                                                 │
│  ┌─────────────────┐  ┌─────────────────┐       │
│  │   PILOTE        │  │  PASSAGER       │       │
│  │   GAUCHE        │  │   DROIT         │       │
│  │                 │  │                 │       │
│  │ ■ COLLECTIF     │  │                 │       │
│  │ ■ CYCLIQUE      │  │                 │       │
│  │ ■ PÉDALES       │  │                 │       │
│  └─────────────────┘  └─────────────────┘       │
│                                                 │
│            TABLEAU DE BORD                      │
│     ┌─────────────────────────────────────┐     │
│     │ ALT │ IAS │ ATT │ COMP │ RPM │ MANI │     │
│     │     │     │     │      │     │      │     │
│     └─────────────────────────────────────┘     │
│                                                 │
└─────────────────────────────────────────────────┘

    TRAIN D'ATTERRISSAGE
   ┌───┐       ┌───┐
   │   │       │   │
   └───┘       └───┘

MOTEUR LYCOMING O-235-N2C (124 ch)
TRANSMISSION PRINCIPALE (Ratio 9.09:1)
```

## Vue Dessus - Configuration

```
ROBINSON R22 - VUE DESSUS
═══════════════════════════

           ROTOR PRINCIPAL
        ┌─────────────────┐
        │   PALE 1   PALE 2│
        │                 │
        │   AVANT         │ ← Direction de vol
        └─────────────────┘

   ROTOR QUEUE
   ┌─────────┐
   │ P1  P2  │ ← Anti-horaire
   └─────────┘

┌─────────────────────────────────────┐
│         COCKPIT BIPLACE             │
├─────────────────────────────────────┤
│  PILOTE   │   PASSAGER              │
│  GAUCHE   │   DROIT                 │
├─────────────────────────────────────┤
│  COMMANDES GAUCHE │ COMMANDES DROITE│
│  COLLECTIF        │                 │
│  CYCLIQUE CENTRE  │                 │
│  PÉDALES PLANCHER │                 │
└─────────────────────────────────────┘

    MOTEUR ARRIÈRE
   ┌─────────────┐
   │ LYCOMING    │
   │ O-235-N2C   │
   │ 124 ch      │
   └─────────────┘
```

## Systèmes Mécaniques - Schéma Fonctionnel

```
SYSTÈME ROTORIQUE R22
══════════════════════

MOTEUR ── TRANSMISSION ── ROTOR PRINCIPAL ── PORTANCE
  │          │                   │
  │          │                   └── Poussee (dissymétrie)
  │          │
  │          └── ROTOR DE QUEUE ── Compensation couple
  │
  └── SYSTÈMES SUPPORT
      ├── Carburant (81.4L)
      ├── Lubrification (3.8L)
      ├── Électrique (12V)
      └── Refroidissement (air)

DÉTAIL TRANSMISSION:
Moteur 2'800 tr/min → Réducteur 9.09:1 → Rotor 309 tr/min
Puissance max: 93 kW (124 ch)
Rendement transmission: 97-98%
```

## Dimensions et Performances

```
DIMENSIONS ROBINSON R22
════════════════════════

LONGUEUR TOTALE    │ 8.76 m
HAUTEUR TOTALE     │ 2.72 m
DIAMÈTRE ROTOR     │ 7.67 m
DIAMÈTRE ROTOR Q   │ 1.42 m
MASSE À VIDE       │ 408 kg
MASSE MAXIMALE     │ 635 kg
CHARGE UTILE       │ 269 kg

PERFORMANCES
════════════
VITESSE CROISIÈRE  │ 170 km/h (93 kt)
VITESSE MAXIMALE   │ 190 km/h (104 kt)
PLAFOND PRATIQUE   │ 4'270 m (14'000 ft)
AUTONOMIE          │ 3.0 h (avec réserves)
TAUX MONTÉE        │ 1'220 ft/min
```

## Schéma des Forces en Vol Stationnaire

```
FORCES EN STATIONNAIRE
═══════════════════════

              PORTANCE (L)
                 ↑
                 │
                 │
                 │
POIDS (W) ←──────○──────→ TRAÎNÉE (D)
                 │
                 │
                 │
              POUSSÉE (T)

ÉQUILIBRE:
Σ Forces verticales = 0: L = W = 5'886 N (600 kg)
Σ Forces horizontales = 0: T = D

CALCUL PORTANCE:
L = ½ × ρ × V² × S × Cl
ρ = 1.225 kg/m³ (niveau mer)
V = vitesse induite (calculée)
S = surface rotor = π × r² = 46 m²
Cl max ≈ 1.2
```

## Vue 3D Simplifiée

```
REPRÉSENTATION 3D ROBINSON R22
═══════════════════════════════

     ROTOR PRINCIPAL (7.67m)
   ┌─────────────────────┐
   │                     │
   └─────────────────────┘

        ROTOR QUEUE
      ┌───────────┐
      │           │
      └───────────┘

   ┌─────────────────────┐
   │   COCKPIT           │
   │  PILOTE   PASSAGER  │
   └─────────────────────┘

     ┌─────────────┐
     │   MOTEUR    │
     │ LYCOMING    │
     │ O-235-N2C   │
     └─────────────┘

     TRAIN ATTERRISSAGE
    ┌───┐       ┌───┐
    │   │       │   │
    └───┘       └───┘
```

## Légende des Couleurs (si applicable)

- 🔵 Rotor principal
- 🟢 Rotor de queue
- 🔴 Moteur et transmission
- 🟡 Cockpit et commandes
- 🟠 Carburant et fluides
- ⚪ Structure générale
