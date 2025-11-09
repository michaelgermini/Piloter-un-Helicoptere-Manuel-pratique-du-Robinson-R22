# Chapitre 4 – Le poste de pilotage du R22

## Tableau de bord annoté

Le cockpit du Robinson R22, bien que compact, concentre toutes les informations essentielles au pilotage. Sa disposition logique facilite la gestion des tâches prioritaires.

### Disposition générale

**Sièges côte à côte** :
- Pilote gauche (commandes prioritaires)
- Passager droit (instruments secondaires)
- Espace réduit : 1.22 m de largeur utile

**Accès et ergonomie** :
- Portes coulissantes (optionnelles)
- Harnais à 4 points avec inertie
- Sièges ajustables en hauteur (±5 cm)
- Repose-pieds réglables

### Instruments primaires (T - Attitude - Heading)

**Horizon artificiel (Attitude Indicator)** :
- Position : Centre haut du panneau
- Fonction : Référence de tangage et roulis
- Échelle : ±90° tangage, ±30° roulis
- Particularité : Cageable manuellement

**Anémomètre (Airspeed Indicator)** :
- Position : Gauche, premier cadran
- Échelle : 0-200 km/h
- Marques colorées : Blanc (50-100 kt), Jaune (100-140 kt), Rouge (140+ kt)
- Précision : ±5 kt

**Altimeter (Altimeter)** :
- Position : Centre gauche
- Unité : Pieds (feet) ou mètres
- Réglage QNH : Molette avant
- Fenêtre secondaire : Tendances

### Instruments moteur et navigation

**Tachymètre rotor (RPM Indicator)** :
- Position : Centre haut
- Échelle : 0-600 tr/min (×100)
- Zone verte : 450-510 tr/min
- Alarme : Voyant rouge >520 tr/min

**Manifold Pressure** :
- Position : Droite du tachymètre
- Unité : Pouces Hg (inches)
- Plage : 10-30 inHg
- Indicateur de puissance moteur

**Température huile (Oil Temperature)** :
- Position : Bas gauche
- Plage : 0-120°C
- Zone normale : 60-100°C
- Alarme : >110°C

**Pression huile (Oil Pressure)** :
- Position : À côté température
- Plage : 0-7 bar
- Zone normale : 2.8-4.1 bar
- Alarme : <2.0 bar ou >5.5 bar

**Compass magnétique** :
- Position : Haut centre
- Type : Bouton flottant
- Précision : ±5°
- Compensation : Nécessaire périodique

**Horloge** :
- Position : Bas centre
- Fonctions : Chrono + temps réel
- Alimentation : Batterie indépendante

## Instruments essentiels (RPM, manifold, altimètre, horizon artificiel)

Quatre instruments forment le "cœur" du pilotage du R22. Leur surveillance continue assure la sécurité du vol.

### RPM : pouls de l'hélicoptère

**Signification** :
- Régime rotor principal (×100 affiché)
- Indicateur direct de la puissance développée
- Stabilité = sécurité

**Zones de fonctionnement** :

| Zone | RPM | Couleur | Signification |
|------|-----|---------|---------------|
| **Verte** | 450-510 | Vert | Fonctionnement normal |
| **Jaune** | 430-450 / 510-520 | Jaune | Attention requise |
| **Rouge** | <430 / >520 | Rouge | Dangereux |

**Gestion pratique** :
- **Stationnaire** : 500-510 tr/min (pleins gaz)
- **Croisière** : 480-500 tr/min
- **Approche** : 500 tr/min (puissance disponible)

⚠️ **Règle d'or** : Jamais en dessous de 430 tr/min en vol. Risque de vortex ring state imminent.

### Manifold Pressure : puissance disponible

**Principe de mesure** :
- Pression absolue dans le collecteur d'admission
- Indicateur de la puissance moteur disponible
- Influence directe sur les performances

**Corrélations pratiques** :

| Régime rotor | Manifold | Puissance approximative |
|--------------|----------|-------------------------|
| 500 tr/min | 28 inHg | 100% (93 kW) |
| 480 tr/min | 24 inHg | 85% (79 kW) |
| 450 tr/min | 20 inHg | 70% (65 kW) |

**Facteurs influençant** :
- Altitude : Diminue avec la densité
- Température : Diminue par dilatation thermique
- Régime moteur : Corrélation directe

### Altimètre : référence verticale

**Principe barométrique** :
- Mesure de pression atmosphérique
- Conversion en altitude via QNH
- Référence pour tous les vols

**Réglages essentiels** :

**QNH (pression au niveau de la mer)** :
- Aéroport de départ : Régler la pression locale
- En route : QNH régional ou 1013.25 hPa (standard)
- Destination : QNH de l'aéroport d'arrivée

**Exemple de calcul** :
```
Altitude vraie = Altitude indiquée + (Température - ISA) × 4 ft/°C/1'000 ft
ISA = 15°C - 2°C/1'000 ft
```

**Erreurs courantes** :
- Oubli de régler le QNH : Erreur de 30 ft par hPa
- Changement de température : 4 ft/°C/1'000 ft
- Non-linéarité : Compression des échelles hautes altitudes

### Horizon artificiel : référence d'attitude

**Instrument gyroscopique** :
- Horizon stabilisé par gyroscope
- Référence inertielle de l'attitude
- Indépendant des facteurs externes

**Interprétation** :

**Tangage (Pitch)** :
- Aile basse = Tangage positif (montée)
- Aile haute = Tangage négatif (descente)
- Échelle : ±90° (rarement utilisé au-delà ±30°)

**Roulis (Roll)** :
- Inclinaison latérale
- Échelle : ±30°
- Limite pratique : ±20° pour le R22

**Erreurs possibles** :
- **Précession** : Erreur progressive (recager toutes les 15 min)
- **Limitation** : Fonctionne seulement si alimenté
- **Référence** : À confirmer avec l'extérieur en VFR

## Les commandes de vol : cyclique, collectif, pédales

Les trois commandes fondamentales du pilotage hélicoptère permettent un contrôle tridimensionnel complet.

### Le collectif : gestion de la puissance

**Position et fonction** :
- Manette gauche (poignée pistolet)
- Contrôle du pas général des pales
- Gestion simultanée : Portance + Puissance

**Course et effets** :

| Position | Angle pas | Effets |
|----------|-----------|--------|
| **Bas** | -10° | Puissance minimale, autorotation |
| **Milieu** | +10° | Vol normal, stationnaire |
| **Haut** | +27° | Puissance maximale, décollage |

**Corrélation RPM** :
- Collectif ↑ → RPM ↓ (compensation automatique requise)
- Collectif ↓ → RPM ↑ (réduction gaz requise)

**Technique de coordination** :
1. Pousser collectif pour plus de puissance
2. Ouvrir gaz pour maintenir RPM
3. Ajuster cyclique pour attitude
4. Coordonner avec pédales

### Le cyclique : contrôle de l'attitude

**Position et ergonomie** :
- Manette centrale (entre les jambes)
- Contrôle du pas différentiel des pales
- Mouvement dans toutes les directions

**Axe de tangage (avant/arrière)** :
- Avant : Tangage positif, accélération
- Arrière : Tangage négatif, décélération
- Course : ±25° (limite ±10° cyclique)

**Axe de roulis (gauche/droite)** :
- Gauche : Inclinaison gauche, virage gauche
- Droite : Inclinaison droite, virage droit
- Précession : 90° dans le sens de rotation

**Sensibilité variable** :
- **Lent** : Près du neutre (précision stationnaire)
- **Rapide** : En bout de course (manoeuvres dynamiques)

### Les pédales : contrôle directionnel

**Position et fonction** :
- Pédales au plancher
- Contrôle du pas rotor de queue
- Compensation du couple moteur

**Effet directionnel** :
- Pédale droite : Nez vers la droite
- Pédale gauche : Nez vers la gauche
- Course : ±20° de pas rotor queue

**Coordination avec le collectif** :
- Collectif ↑ → Plus de couple → Pédales requises
- Collectif ↓ → Moins de couple → Pédales relâchées

**Technique de tenue de cap** :
1. Observer dérive du nez
2. Appliquer pédale opposée progressivement
3. Maintenir pression légère
4. Ajuster selon vitesse et puissance

## Équipement de sécurité et accessoires

### Instruments de sécurité

**Avertisseurs sonores** :
- Bip rotor bas (< 430 tr/min)
- Alarme température (> 110°C)
- Alarme pression (< 2 bar)

**Voyants lumineux** :
- Rotor RPM (rouge si hors limites)
- Starter (engagement moteur)
- Alternateur (charge batterie)

### Équipement de communication

**Radio VHF** :
- Fréquences 118-136 MHz
- Puissance 5-10 W
- Port micro-casque standard

**Transpondeur** :
- Mode A/C/S disponible
- Altitude automatique (option)
- Squawk codes d'urgence

### Instruments optionnels

**GPS portatif** :
- Navigation par satellite
- Base de données aéronautiques
- Fonctions d'approche

**Enregistreur de vol** :
- Données moteur et vol
- Analyse post-vol
- Maintenance prédictive

## Synthèse du chapitre

Le poste de pilotage du R22, bien que simple dans sa conception, offre toutes les informations nécessaires au pilotage sécurisé. Les quatre instruments essentiels (RPM, manifold, altimètre, horizon) forment le minimum requis pour le vol, complétés par les trois commandes fondamentales.

La maîtrise de cet environnement confiné exige une organisation rigoureuse des tâches et une surveillance continue des paramètres critiques.

---

**Évaluation** :
- Pouvez-vous nommer les quatre instruments essentiels du R22 ?
- Quelle est la fonction de chaque commande de vol ?
- Comment gérer la coordination collectif-pédales ?

**Exercice pratique** :
En stationnaire, votre RPM indique 495 tr/min. Que devez-vous faire ? Si le manifold indique 26 inHg en croisière à 4'000 ft, quelle puissance approximative développez-vous ?

**Pour aller plus loin** :
- Entraînez-vous sur un simulateur R22
- Étudiez les procédures d'urgence instrumentées
- Comparez avec d'autres cockpits d'hélicoptères
