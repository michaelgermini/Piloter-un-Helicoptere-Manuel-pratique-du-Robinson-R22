# Chapitre 4 bis – Détail des instruments du tableau de bord R22

## Vue d'ensemble du cockpit avec schémas

![Tableau de bord R22 - Vue d'ensemble](assets/tableau-bord-ascii.md)

Le tableau de bord du Robinson R22 intègre tous les instruments essentiels au pilotage sécurisé. Chaque cadran joue un rôle spécifique dans le contrôle de l'attitude, de la trajectoire et de la santé mécanique de l'appareil.

## 1. Indicateur d'assiette (Horizon artificiel)

```
┌─────────────────┐
│   HORIZON       │
│   ARTIFICIEL    │
│                 │
│    █████████    │ ← Ligne d'horizon
│   ██        ██  │
│  █            █ │
│ █    AVION     █ │
│  █            █ │
│   ██        ██  │
│    █████████    │
│                 │
│ ±90° TANGAGE   │
│ ±30° ROULIS     │
└─────────────────┘
```

**Fonction principale** : Montre si l'hélicoptère est en montée, descente ou inclinaison gauche/droite.

**Utilisation** : Essentiel en vol sans repère visuel (IMC - Instrument Meteorological Conditions).

**Caractéristiques R22** :
- Échelle : ±90° tangage, ±30° roulis
- Cageable manuellement pour recalage
- Alimenté par gyroscope
- Référence primaire d'attitude

**Lecture** :
- Aile basse = Tangage positif (montée)
- Aile haute = Tangage négatif (descente)
- Inclinaison latérale = Roulis

⚠️ **Attention** : Recager toutes les 15 minutes pour compenser la précession gyroscopique.

## 2. Altimètre

```
┌─────────────────┐
│   ALTIMETER     │
│                 │
│     2 5 0 0     │ ← Altitude en pieds
│    ██████████   │
│   ██        ██  │
│  █     ■      █ │ ← Aiguille des 100 ft
│ █              █ │
│  █            █ │
│   ██        ██  │
│    █████████    │
│                 │
│  QNH  1 0 1 3   │ ← Réglage pression
└─────────────────┘
```

**Fonction principale** : Indique l'altitude au-dessus du niveau de la mer (en pieds).

**Réglage essentiel** : Le pilote règle la pression atmosphérique locale (QNH) avant le vol.

**Caractéristiques R22** :
- Échelle : 0-30'000 pieds
- Précision : ±20 pieds
- Unité : Pieds (feet) ou mètres
- Fenêtre secondaire : Tendances

**Utilisation** :
- **QNH** : Pression au niveau de la mer (réglée à l'aéroport)
- **QFE** : Pression au niveau du terrain (zéro à l'atterrissage)

**Erreurs courantes** :
- Oubli de régler QNH : Erreur de 30 ft par hPa
- Changement température : 4 ft/°C/1'000 ft

## 3. Variomètre (VSI - Vertical Speed Indicator)

```
┌─────────────────┐
│     VARIOMETER  │
│   VERTICAL SPEED│
│                 │
│       ▲         │ ← Montée
│      ███        │
│     █████       │
│    ███████      │
│   █████████     │
│  ███████████    │
│ █████████████   │
│███████████████  │
│      ███        │ ← Zéro
│       ▼         │ ← Descente
│                 │
│  0 ±2000 FT/MIN │
└─────────────────┘
```

**Fonction principale** : Montre la vitesse verticale, c'est-à-dire le taux de montée ou descente (en pieds/minute).

**Caractéristiques R22** :
- Échelle : ±2'000 ft/min
- Précision : ±100 ft/min
- Type : Pression différentielle

**Interprétation** :
- Aiguille vers le haut = Montée
- Aiguille vers le bas = Descente
- Zéro = Vol horizontal

**Applications** :
- Contrôle précision altitude
- Approches stabilisées
- Montées/descentes contrôlées

## 4. Indicateur de vitesse (Airspeed Indicator)

```
┌─────────────────┐
│ AIRSPEED INDICATOR│
│                 │
│     1 2 0       │ ← Vitesse en nœuds
│    ██████████   │
│   ██   ■    ██  │ ← Marques colorées
│  █    ███    █ │
│ █     ███     █ │
│  █    ███    █ │
│   ██   ■    ██  │
│    ██████████   │
│                 │
│ BLANC JAUNE ROUGE│ ← Zones de vitesse
└─────────────────┘
```

**Fonction principale** : Donne la vitesse horizontale en nœuds (1 nœud ≈ 1,85 km/h).

**Importance critique** : Très important pour éviter le décrochage ou le "vortex ring state".

**Marques colorées R22** :
- **Blanc** : 50-100 kt (vitesse normale)
- **Jaune** : 100-140 kt (caution)
- **Rouge** : >140 kt (VNO - Never Exceed)

**Limites R22** :
- VNO (max continu) : 140 kt
- VNO (structurel) : 190 km/h

**Risques** :
- Trop lent : Vortex ring state
- Trop rapide : Charges structurales excessives

## 5. Compas magnétique / Direction gyroscopique

```
┌─────────────────┐
│   COMPASS       │
│  MAGNETIC       │
│                 │
│     ▲ N         │
│   ◄W    E►      │
│     ▼ S         │
│                 │
│    0 9 0        │ ← Cap actuel
│   ██████████    │
│  ██   ■    ██   │
│ █     │      █  │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│   GYRO HDG      │ ← Direction gyro
└─────────────────┘
```

**Fonction principale** : Donne le cap de vol (orientation par rapport au nord).

**Double système** :
- **Compas magnétique** : Référence vraie (sujet aux erreurs)
- **Direction gyroscopique** : Stabilisé (recagé sur compas)

**Caractéristiques** :
- Échelle : 360°
- Précision : ±5°
- Type : Bouton flottant (compas)

**Utilisation** :
- Navigation VFR
- Référence de cap
- Coordination virages

---

## ⚙️ Section intermédiaire – Instruments moteur

Ces cadrans surveillent la santé du moteur Lycoming et du rotor :

## 6. Tachymètre double (RPM moteur / RPM rotor)

```
┌─────────────────┐
│   TACHYMETER    │
│   DOUBLE RPM    │
│                 │
│ MTR  2 8 0 0   │ ← RPM moteur (×100)
│ ROT  5 0 5     │ ← RPM rotor
│   ██████████    │
│  ██   ■    ██   │
│ █     │      █  │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│ MTR ROT SYNC    │ ← Synchronisation
└─────────────────┘
```

**Fonction principale** : Cadran à deux aiguilles pour surveiller les régimes moteur et rotor.

**Détail** :
- **Une aiguille** : Régime moteur (en % de la puissance nominale)
- **Une aiguille** : Régime rotor

**Synchronisation** : Les deux doivent rester synchronisées (≈ 100 % en vol).

**Valeurs normales R22** :
- Moteur : 2'800 tr/min (100%)
- Rotor : 500 tr/min (synchronisé)
- Alarme : <430 tr/min rotor = Danger immédiat

## 7. Pression d'huile

```
┌─────────────────┐
│ OIL PRESSURE    │
│   BAR           │
│                 │
│     3 . 8       │ ← Pression actuelle
│    ██████████   │
│   ██   ■    ██  │
│  █     █      █ │
│ █       █      █ │
│  █     █      █ │
│   ██   ■    ██  │
│    ██████████   │
│                 │
│ 2.8-4.1 BAR     │ ← Zone verte
└─────────────────┘
```

**Fonction principale** : Indique la pression dans le circuit de lubrification moteur.

**Action critique** : Si elle chute, il faut couper le moteur rapidement.

**Valeurs R22** :
- Normal : 2.8-4.1 bar
- Alarme : <2.0 bar (rouge)
- Maximum : >5.5 bar (jaune)

**Causes pannes** :
- Niveau huile bas
- Pompe défaillante
- Fuite circuit

## 8. Température d'huile

```
┌─────────────────┐
│ OIL TEMPERATURE │
│   °C            │
│                 │
│     8 5         │ ← Température actuelle
│    ██████████   │
│   ██   ■    ██  │
│  █     █      █ │
│ █       █      █ │
│  █     █      █ │
│   ██   ■    ██  │
│    ██████████   │
│                 │
│ 60-100°C        │ ← Zone normale
└─────────────────┘
```

**Fonction principale** : Montre la température du lubrifiant moteur.

**Risque** : Trop chaud = risque de surchauffe / grippage.

**Valeurs R22** :
- Normal : 60-100°C
- Alarme : >110°C
- Démarrage : <80°C requis

**Gestion** :
- Refroidissement par convection
- Surveillance continue
- Réduction puissance si chaud

## 9. Température des gaz d'échappement (EGT)

```
┌─────────────────┐
│   EGT           │
│EXHAUST GAS TEMP │
│   °C            │
│                 │
│    6 5 0        │ ← Température actuelle
│   ██████████    │
│  ██   ■    ██   │
│ █     │      █  │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│ <700°C          │ ← Limite normale
└─────────────────┘
```

**Fonction principale** : Sert à régler le mélange air-carburant.

**Alerte** : Trop élevée = mélange trop pauvre (danger).

**Utilisation** :
- Réglage richesse mélange
- Peak EGT pour économie
- Surveillance surchauffe

**Limites** :
- Normal : <700°C
- Alarme : >700°C continu

## 10. Température du cylindre (CHT)

```
┌─────────────────┐
│   CHT           │
│CYLINDER HEAD TEMP│
│   °C            │
│                 │
│    1 8 0        │ ← Température max
│   ██████████    │
│  ██   ■    ██   │
│ █     │      █  │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│ <200°C          │ ← Limite normale
└─────────────────┘
```

**Fonction principale** : Indique la température des têtes de cylindres.

**Rôle** : Permet de contrôler le refroidissement moteur.

**Surveillance** :
- Refroidissement air forcé
- Ventilation capot
- Réduction puissance si nécessaire

**Limites** :
- Normal : <200°C
- Critique : >220°C

## 11. Pression de carburant

```
┌─────────────────┐
│ FUEL PRESSURE   │
│   BAR           │
│                 │
│    0 . 3        │ ← Pression actuelle
│   ██████████    │
│  ██   ■    ██   │
│ █     │      █  │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│ 0.2-0.3 BAR     │ ← Zone normale
└─────────────────┘
```

**Fonction principale** : Indique la pression d'alimentation du carburant vers le moteur.

**Système R22** :
- Pompe mécanique
- Filtre intégré
- Pression : 0.2-0.3 bar

**Pannes possibles** :
- Pompe défaillante
- Filtre obstrué
- Fuite circuit

## 12. Jauge à carburant

```
┌─────────────────┐
│   FUEL QUANTITY │
│   LITRES        │
│                 │
│    6 5 . 0      │ ← Quantité restante
│   ██████████    │
│  ██   ■    ██   │
│ █     ███     █ │
│  ██   ■    ██   │
│   ██████████    │
│                 │
│ RESERVE 9.1L    │ ← Réserve minimale
└─────────────────┘
```

**Fonction principale** : Indique la quantité de carburant restante dans le réservoir.

**Capacité R22** : 81.4 L (réserve 9.1 L)

**Consommation** : Environ 35 L/h selon puissance

**Calculs** :
- Autonomie = Carburant ÷ Consommation
- Réserve = 30 minutes minimum

---

## 💡 Section inférieure – Commandes et voyants

C'est ici qu'on trouve les interrupteurs et alertes :

## 13. Voyants lumineux (Annunciator Panel)

```
┌─────────────────────────────────────┐
│        ANNUNCIATOR PANEL            │
│                                     │
│  □ LOW RPM          □ CLUTCH        │
│  □ MR TEMP          □ MR CHIP       │
│  □ LOW FUEL         □ GENERATOR     │
│  □ LOW VOLT         □ OIL PRESS     │
│  □ HIGH TEMP        □ START         │
│                                     │
│  ROUGE = DANGER     JAUNE = ATTENTION│
│  VERT = NORMAL                       │
└─────────────────────────────────────┘
```

**Fonction principale** : Alertes lumineuses pour diverses conditions.

**Voyants principaux** :
- **LOW RPM** : Régime rotor trop bas
- **CLUTCH** : Embrayage actif
- **MR TEMP/CHIP** : Surchauffe ou particules huile rotor
- **LOW FUEL** : Carburant bas
- **GENERATOR** : Alternateur défaillant
- **OIL PRESS** : Pression huile basse

**Codes couleur** :
- 🔴 Rouge : Dangers immédiats
- 🟡 Jaune : Conditions dégradées
- 🟢 Vert : Fonctionnement normal

## 14. Commandes de démarrage et systèmes électriques

```
┌─────────────────────────────────────┐
│      COMMANDES ÉLECTRIQUES          │
│                                     │
│  [START] Bouton démarreur moteur    │
│  [CLUTCH] Embraye/débraye rotor     │
│  [ALT] Alternateur ON/OFF           │
│  [MAGS] Magnétos L/BOTH/R           │
│  [LIGHTS] Éclairage navigation      │
│  [AVIONICS] Systèmes électroniques  │
│  [MASTER] Alimentation générale     │
│                                     │
└─────────────────────────────────────┘
```

**Commandes essentielles** :
- **START** : Démarreur moteur (max 30 sec)
- **CLUTCH** : Connecte moteur au rotor
- **ALT** : Charge batterie via alternateur
- **MAGS** : Système d'allumage (Left/Both/Right)
- **LIGHTS/AVIONICS** : Interrupteurs divers

## 15. Horloge numérique et radio

```
┌─────────────────────────────────────┐
│         AFFICHAGE CENTRAL           │
│                                     │
│  TIME: 14:32:15   FLT: 02:15:30    │
│  COM1: 118.725    COM2: 121.500    │
│  NAV1: 110.300    NAV2: 117.950    │
│                                     │
│  Horloge numérique + Radio intégrée │
└─────────────────────────────────────┘
```

**Fonction principale** : Afficheur central utilisé pour le temps de vol et les fréquences COM.

**Affichage** :
- **TIME** : Heure actuelle
- **FLT** : Temps de vol total
- **COM1/COM2** : Fréquences communication
- **NAV1/NAV2** : Fréquences navigation (optionnel)

## 16. Collectif et cyclique

![Commandes de vol](assets/commandes-schema.md)

**Collectif** (levier gauche) : Contrôle la portance générale (altitude).

**Cyclique** (manche central) : Contrôle la direction du vol (avant/arrière/gauche/droite).

**Coordination** : Les trois commandes travaillent ensemble pour un vol harmonieux.

---

## 📋 Check-list des instruments

### Pré-vol
- [ ] Tous instruments dans zones vertes
- [ ] Horizon artificiel cagéré
- [ ] Altimètre QNH réglé
- [ ] Compas synchronisé
- [ ] Réserves carburant vérifiées

### En vol
- [ ] Surveillance continue RPM rotor
- [ ] Températures dans limites
- [ ] Pressions normales
- [ ] Voyants lumineux : Aucun rouge/jaune

### Post-vol
- [ ] Instruments remis à zéro
- [ ] Anomalies notées
- [ ] Maintenance préventive planifiée

## 🔧 Dépannage instruments

### Horizon artificiel
- Problème : Aiguille bloquée
- Cause : Gyro défaillant
- Action : Utiliser repères visuels

### Altimètre
- Problème : Lecture erronée
- Cause : QNH incorrect
- Action : Recaler sur altitude connue

### Instruments moteur
- Problème : Alarmes répétées
- Cause : Capteurs défaillants
- Action : Atterrissage immédiat, maintenance

## Synthèse du chapitre

Le tableau de bord du R22 concentre une multitude d'informations essentielles au pilotage sécurisé. Chaque instrument joue un rôle spécifique dans la surveillance de l'attitude, de la trajectoire et de la santé mécanique.

La maîtrise de ces instruments permet une prise de décision rapide et précise, élément crucial de la sécurité du vol hélicoptère.

---

**Évaluation** :
- [ ] Identification des instruments principaux
- [ ] Compréhension des fonctions de chaque cadran
- [ ] Connaissance des limites et alarmes

**Exercice pratique** :
En vol de croisière, votre altimètre indique 3'500 ft, le variomètre -200 ft/min, et le tachymètre rotor 485 tr/min. Analysez la situation et décrivez les actions à prendre.

**Pour aller plus loin** :
- Étudier le manuel de vol Robinson R22
- Pratiquer sur simulateur les lectures instruments
- Comparer avec autres hélicoptères
