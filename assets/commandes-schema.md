# Schéma des Commandes de Vol - Robinson R22

## Vue d'ensemble des Commandes

```
COCKPIT ROBINSON R22 - CONFIGURATION BIPLACE CÔTE À CÔTE
═════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────┐
│                    PILOTE GAUCHE                    │
├─────────────────────────────────────────────────────┤
│  ┌─────────────────┐  ┌─────────────────────────┐   │
│  │   COLLECTIF     │  │   CYCLIQUE (CENTRE)     │   │
│  │   (GAUCHE)      │  │                         │   │
│  │                 │  │   ■ AVANT/ARRIÈRE       │   │
│  │ ■ HAUT/BAS      │  │   ■ GAUCHE/DROITE       │   │
│  │ ■ PAS GÉNÉRAL  │  │   ■ ROULIS + TANGAGE    │   │
│  │ ■ PUISSANCE     │  │   ■ COURSE ±25°        │   │
│  │ ■ VERROUILLAGE │  │   ■ PRÉCESSION 90°      │   │
│  │                 │  │   ■ FRICTION AJUSTABLE │   │
│  └─────────────────┘  └─────────────────────────┘   │
│                                                     │
│                PÉDALES AU PLANCHER                  │
│       ┌─────────────────────────────────────┐       │
│       │  GAUCHE ←───○───→ DROITE            │       │
│       │                                     │       │
│       │ ■ COMPENSATION COUPLE MOTEUR        │       │
│       │ ■ PAS ROTOR QUEUE ±20°              │       │
│       │ ■ LACET GAUCHE/DROITE               │       │
│       │ ■ FRICTION FIXE                     │       │
│       └─────────────────────────────────────┘       │
└─────────────────────────────────────────────────────┘
```

## Détail des Fonctions

### COLLECTIF (Manette Gauche)

```
FONCTION: Gestion de la portance et puissance
POSITION: Poignet gauche, manette pistolet
COURSE: -10° (bas) à +27° (haut)

ACTIONS ASSOCIÉES:
├── HAUT (+) : Plus de portance, plus de puissance
├── BAS (-)  : Moins de portance, moins de puissance
├── COORDINATION: Gaz moteur pour maintenir RPM
└── VERROUILLAGE: Crochet anti-débrayage

EFFETS:
├── Rotor: Augmente le pas collectif
├── Moteur: Gaz automatique (compensation)
├── RPM: Maintien constant par pilote
└── Performance: Portance + puissance simultanées
```

### CYCLIQUE (Manette Centrale)

```
FONCTION: Contrôle de l'attitude et direction
POSITION: Entre les jambes, manette centrale
COURSE: ±25° (tangage) × ±30° (roulis)

COMMANDES:
├── AVANT: Tangage positif (montée)
├── ARRIÈRE: Tangage négatif (descente)
├── GAUCHE: Roulis gauche (virage gauche)
└── DROITE: Roulis droite (virage droite)

PRÉCESSION GYROSCOPIQUE:
├── Force appliquée côté gauche
├── Effet 90° plus tard (avant)
├── Compensation automatique
└── Sensibilité variable selon vitesse
```

### PÉDALES (Au Plancher)

```
FONCTION: Compensation couple et contrôle directionnel
POSITION: Plancher cockpit, commande pied
COURSE: ±20° de pas rotor queue

ACTIONS:
├── PÉDALE DROITE: Nez vers droite
├── PÉDALE GAUCHE: Nez vers gauche
├── COORDINATION: Avec collectif
└── FRICTION: Fixe (non ajustable)

COMPENSATION COUPLE:
├── Collectif ↑ → Couple ↑ → Pédales requises
├── Collectif ↓ → Couple ↓ → Pédales relâchées
├── Vitesse ↑ → Compensation accrue
└── Timing: Pédales après collectif
```

## Schéma de Coordination

```
SÉQUENCE TYPique DÉCOLLAGE:
═══════════════════════════

1. COLLECTIF: Lever progressivement (+ portance)
2. GAZ: Ouvrir pour maintenir RPM rotor
3. CYCLIQUE: Maintenir attitude droite
4. PÉDALES: Ajuster pour cap constant

COORDINATION CONTINUE:
├── Collectif ↔ Gaz (RPM constant)
├── Cyclique ↔ Pédales (équilibre latéral)
├── Anticipation (précession rotor)
└── Douceur (pas de mouvements brusques)
```

## Instruments de Référence

```
TABLEAU DE BORD - INSTRUMENTS ESSENTIELS
═════════════════════════════════════════

┌─────────────┬─────────────┬─────────────┬─────────────┐
│   ALTITUDE  │  VITESSE    │   ATTITUDE  │ DIRECTION   │
│  ALTIMETER  │ ANEMOMETER  │ HORIZON ART │  COMPASS    │
├─────────────┼─────────────┼─────────────┼─────────────┤
│ 0-30'000 ft │ 0-200 kt    │ ±90°/±30°  │ 360°        │
│ QNH réglage │ Blanc/Jaune │ Cageable    │ Magnétique  │
│ pieds/mètres │ Rouge >140kt│ Référence   │ Bouton      │
└─────────────┴─────────────┴─────────────┴─────────────┘

┌─────────────┬─────────────┬─────────────┬─────────────┐
│    PUISSANCE│   MOTEUR    │   TEMPS     │ ALT SECONDE │
│   RPM ROTOR │ MANIFOLD PR │   HORLOGE   │   ALTIMETER │
├─────────────┼─────────────┼─────────────┼─────────────┤
│ 0-600 (×100)│ 10-30 inHg  │ H:M:S       │ 0-30'000 ft │
│ Vert 450-510│ Indicateur  │ Chrono      │ Tendances   │
│ Rouge <430  │ 28" = 100%  │ Batterie    │ QNH local   │
│ >520 tr/min │             │             │             │
└─────────────┴─────────────┴─────────────┴─────────────┘

┌─────────────┬─────────────┬─────────────┐
│ TEMP HUILE  │ PRESS HUILE │ CARBURANT  │
├─────────────┼─────────────┼─────────────┤
│ 0-120°C     │ 0-7 bar     │ 0-82 L     │
│ Vert 60-100 │ Vert 2.8-4.1│ Jaune 9-15 │
│ Rouge >110  │ Rouge <2.0  │ Rouge <9   │
│             │ >5.5        │            │
└─────────────┴─────────────┴─────────────┘
```

## Check-list Visuelle des Commandes

```
PRÉ-DÉMARRAGE:
□ Collectif: Bas, verrouillé
□ Cyclique: Centré, friction ON
□ Pédales: Centrées
□ Instruments: Testés

APRÈS DÉMARRAGE:
□ Test collectif: Course complète, RPM stable
□ Test cyclique: Mouvements, retour centre
□ Test pédales: Déplacements rotor queue
□ Trim: Réglage neutre

EN VOL:
□ Coordination collective/gaz
□ Anticipation précession
□ Pédales douces continues
□ Corrections progressives
```
