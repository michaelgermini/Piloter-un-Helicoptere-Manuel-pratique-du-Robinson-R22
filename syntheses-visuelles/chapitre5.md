# Synthèse Visuelle - Chapitre 5 : Les systèmes du R22

## 🔄 Transmission et rotor

```
BOÎTE DE VITESSES         ROTOR PRINCIPAL           ROTOR DE QUEUE
├── Rapport 9.09:1       ├── 2 pales Al 6061-T6   ├── 2 pales composite
├── Rendement 97-98%     ├── Diamètre 7.67m       ├── Diamètre 1.42m
├── Lubrification Carter ├── Pas -10°/+27°       ├── RPM 2'240 tr/min
├── Temp 60-100°C       ├── RPM 500 max          ├── Poussée 1'100N
└── Pression 2.8-4.1 bar └── Profil NACA 23012    └── Efficacité 65-70%
```

## ⛽ Circuit carburant

```
RÉSERVOIR 81.4L          POMPE INJECTION          FILTRES
├── 58.6 kg (0.72kg/L)  ├── Mécanique directe    ├── Admission
├── Jauge électrique     ├── Carburateur MA4-5   ├── Séparation eau
├── Réserve 30 min      ├── Enrichisseur auto    └── Sécurité anti-feu
└── Autonomie 2.4-3h    └── Pression 0.2-0.3 bar

CALCULS:
Temps vol = (Carburant - Réserve) / Consommation
Ex: (70L - 9.1L) / 25L/h = 2.44h
```

## 🛢️ Lubrification

```
CARTER HUMIDE 3.8L       POMPE À ENGRENAGES       REFROIDISSEUR AIR
├── SAE 15W-50          ├── Pression 2.8-4.1 bar ├── Efficacité 80%
├── Additifs anti-usure ├── Température 60-100°C ├── Huile propre
└── Changement 50h      └── Alarme >110°C        └── Spectrométrie option

MAINTENANCE:
- Changement: 50h ou annuel
- Filtre: Remplacement 100h
- Analyse: Spectrométrie recommandée
```

## ⚙️ Commandes hydrauliques

```
CYCLIQUE MÉCANIQUE         COLLECTIF MÉCANIQUE        PÉDALES MÉCANIQUE
├── Tiges push-pull       ├── Câbles Bowden         ├── Tiges rigides
├── Course ±10° pales     ├── Course -10°/+27°      ├── Course ±20° queue
├── Précession compensée  ├── Verrouillage crochet  ├── Friction nulle
└── Deadzone minimale     └── Coordination RPM       └── Centrage fort
```

## 📊 Instruments et alarmes

```
TACHO ROTOR              MANIFOLD                 TEMP HUILE
├── RPM ×100 affiché     ├── Pouces Hg            ├── °C
├── Vert 450-510         ├── 10-30 inHg           ├── 0-120°C
├── Alarme >520          ├── Indicateur puissance └── Alarme >110°C
└── Précision ±1         └── 28 inHg = 100%

PRESSION HUILE           ALARMES SONORES          VOYANTS LUMINEUX
├── 0-7 bar             ├── Buzzer RPM <430      ├── Rouge: Dangers
├── Normal 2.8-4.1      ├── Buzzer temp >110°C   ├── Jaune: Avertissements
├── Alarme <2.0 bar     ├── Cloche pression      └── Vert: Normal
└── Alarme >5.5 bar     └── Continue/intermittent
```

## 🔧 Maintenance 50/100h

```
50 HEURES:
- Bougies: Vérification écartement
- Filtres air: Nettoyage
- Batterie: Charge et électrolyte
- Huile: Changement

100 HEURES:
- Bougies: Remplacement
- Filtres huile: Remplacement
- Câbles commandes: Tension
- Rotor: Équilibrage dynamique
```

## 📋 Évaluation chapitre

### Systèmes maîtrisés
- [ ] Transmission et rotors
- [ ] Carburant et lubrification
- [ ] Commandes et instruments

### Surveillance continue
1. Température huile 60-100°C
2. Pression huile 2.8-4.1 bar
3. RPM rotor 450-510 tr/min
