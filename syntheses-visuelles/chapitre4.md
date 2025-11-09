# Synthèse Visuelle - Chapitre 4 : Le poste de pilotage du R22

## 🕹️ Instruments essentiels (T-Attitude-Heading)

```
HORIZON ARTIFICIEL     ANÉMOMÈTRE         ALTIMÈTRE
├── Tangage ±90°      ├── 0-200 km/h     ├── Pieds/mètres
├── Roulis ±30°       ├── Marques VNO    ├── QNH réglage
├── Cageable          ├── Précision ±5kt ├── QFE/QNH
└── Référence gyro    └── Blanc 50-100kt └── Jaune 100-140kt

TACHO RPM            MANIFOLD          TEMPÉRATURE HUILE
├── 0-600 (×100)     ├── 10-30 inHg    ├── 0-120°C
├── Zone verte 450-510├── Indicateur puissance ├── Normale 60-100°C
├── Alarme >520      └── 28 inHg = 100% └── Alarme >110°C
└── RPM rotor réel   └── 24 inHg = 85%
```

## 🎛️ Les trois commandes

```
COLLECTIF (GAUCHE)          CYCLIQUE (CENTRE)          PÉDALES (PLANCHER)
├── Pas général ±17°       ├── Pas différentiel ±10° ├── Pas rotor queue ±20°
├── Portance + puissance   ├── Attitude tangage/roulis├── Compensation couple
├── RPM ↓ quand ↑         ├── Précession 90°        ├── Poussée latérale
├── Coordination gaz       ├── Course ±25°           ├── Friction nulle
└── Verrouillage rotor     └── Sensibilité variable    └── Pressions légères
```

## 🔧 Système électrique et sécurité

```
BATTERIE 12V 25Ah          ALTERNATEUR 40A          FUSIBLES PROTECTIONS
├── Démarrage              ├── Charge avionique      ├── 5-15A circuits
├── Instruments secours    ├── Voyant vert ON        ├── Reset automatique
├── Autonomie 30 min       └── Alternateur défaillant ├── Parasurtenseurs
└── Tension >12.5V         └── Charge 25-35A

CONSOMMATION MOYENNE:
Instruments de base: 5-8A
Radio + transpondeur: 2-3A
GPS + éclairage: 1-2A
Total croisière: 8-12A
```

## 📋 Évaluation chapitre

### Maîtrise cockpit
- [ ] Instruments essentiels identifiés
- [ ] Fonctions commandes comprises
- [ ] Gestion électrique maîtrisée

### Procédures clés
1. RPM rotor maintien 500 tr/min
2. Manifold pression 22-24 inHg cruise
3. Coordination collectif-pédales
