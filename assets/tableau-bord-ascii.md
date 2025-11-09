# Tableau de Bord Robinson R22 - Schéma ASCII

```
╔══════════════════════════════════════════════════════════════════════════════╗
║                          TABLEAU DE BORD ROBINSON R22                       ║
║                          Configuration Biplace Côté à Côté                 ║
╚══════════════════════════════════════════════════════════════════════════════╝

┌─────────────────────────────────────────────────────────────────────────────┐
│                             PANNEAU PRINCIPAL                               │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐         │
│  │ ALTITUDE    │  │ VITESSE AIR│  │ HORIZON     │  │ COMPASS     │         │
│  │  ALTIMETER  │  │ ANEMOMETER │  │ ARTIFICIEL  │  │ MAGNETIQUE  │         │
│  │   0-30'000  │  │  0-200 kt  │  │ ATTITUDE    │  │   360°      │         │
│  │   pieds     │  │            │  │ INDICATOR   │  │             │         │
│  │             │  │  Blanc     │  │             │  │             │         │
│  │   [QNH]     │  │ 50-100 kt  │  │  ±90°/±30°  │  │             │         │
│  │             │  │  Jaune     │  │             │  │             │         │
│  │             │  │100-140 kt  │  │             │  │             │         │
│  │             │  │  Rouge     │  │             │  │             │         │
│  │             │  │  140+ kt   │  │             │  │             │         │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘         │
│                                                                             │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐         │
│  │   TACHO     │  │  MANIFOLD  │  │   HORLOGE   │  │   ALTI      │         │
│  │   ROTOR     │  │  PRESSURE  │  │             │  │ SECONDAIRE  │         │
│  │   RPM       │  │   inHg     │  │   [H:M:S]   │  │  ALTITUDE   │         │
│  │  0-600      │  │ 10-30      │  │             │  │             │         │
│  │  (×100)     │  │            │  │             │  │             │         │
│  │             │  │            │  │             │  │             │         │
│  │  Vert       │  │            │  │             │  │             │         │
│  │450-510 tr/min│  │            │  │             │  │             │         │
│  │  Jaune      │  │            │  │             │  │             │         │
│  │430-450/     │  │            │  │             │  │             │         │
│  │510-520      │  │            │  │             │  │             │         │
│  │  Rouge      │  │            │  │             │  │             │         │
│  │   <430      │  │            │  │             │  │             │         │
│  │    >520     │  │            │  │             │  │             │         │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘         │
│                                                                             │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                          │
│  │ TEMP HUILE  │  │ PRESS HUILE│  │  CARBURANT │                          │
│  │   °C        │  │   bar       │  │   litres   │                          │
│  │  0-120      │  │  0-7        │  │   0-82     │                          │
│  │             │  │             │  │            │                          │
│  │   Vert      │  │   Vert      │  │   Jaune    │                          │
│  │ 60-100°C    │  │ 2.8-4.1 bar │  │ 9-15 L    │                          │
│  │   Rouge     │  │   Rouge     │  │   Rouge    │                          │
│  │   >110°C    │  │   <2.0      │  │   <9 L     │                          │
│  │             │  │    >5.5     │  │            │                          │
│  └─────────────┘  └─────────────┘  └─────────────┘                          │
│                                                                             │
│                    ┌───────────────────┐                                   │
│                    │    VOYANTS        │                                   │
│                    │   LUMINEUX        │                                   │
│                    ├───────────────────┤                                   │
│                    │ □ Rotor RPM       │                                   │
│                    │ □ Température     │                                   │
│                    │ □ Pression huile  │                                   │
│                    │ □ Alternateur     │                                   │
│                    │ □ Starter         │                                   │
│                    │ □ Réserve carb    │                                   │
│                    └───────────────────┘                                   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────────┐
│                           COMMANDES DE VOL                                  │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│        COLLECTIF (GAUCHE)                   CYCLIQUE (CENTRE)               │
│   ┌─────────────────────────┐       ┌─────────────────────────┐           │
│   │    MANETTE POIGNET      │       │   MANETTE AVANT/ARRIÈRE │           │
│   │                         │       │   GAUCHE/DROITE         │           │
│   │  ■ Verrouillage rotor   │       │                         │           │
│   │  ■ Gaz moteur           │       │  ■ Précession 90°       │           │
│   │  ■ Mélange              │       │  ■ Course ±25°          │           │
│   │  ■ Choke                │       │  ■ Friction ajustable   │           │
│   └─────────────────────────┘       └─────────────────────────┘           │
│                                                                             │
│                          PÉDALES (AU PLANCHER)                              │
│                    ┌─────────────────────────────┐                         │
│                    │ GAUCHE ←───────○───────→ DROITE │                         │
│                    │      Compensation couple         │                         │
│                    │      Course ±20° rotor queue     │                         │
│                    └─────────────────────────────┘                         │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

## Légende des Couleurs et Zones

```
VERT   : Fonctionnement normal
JAUNE  : Attention requise
ROUGE  : Dangereux - Action immédiate
BLANC  : Zones de vol normal (vitesse air)
NOIR   : Échelles et graduations
```

## Configuration Typique en Vol

```
ALTITUDE     : 2'500 ft     VITESSE AIR : 110 kt
RPM ROTOR    : 495 tr/min   MANIFOLD    : 24 inHg
TEMP HUILE   : 85°C         PRESS HUILE : 3.8 bar
CARBURANT    : 65 L         COMPASS     : 180°
HORIZON      : Centré       QNH         : 1020 hPa
```

## Instruments Essentiels (Rappel)

**RPM Rotor** : Indicateur critique de puissance
**Manifold Pressure** : Pression absolue moteur
**Altimeter** : Altitude barométrique
**Horizon Artificiel** : Référence d'attitude

## Alarmes et Voyants

- **Bip continu** : RPM rotor <430 tr/min
- **Bip intermittent** : Température >110°C
- **Cloche** : Pression huile basse
- **Voyants rouges** : Dangers immédiats
- **Voyants jaunes** : Conditions dégradées
