# Chapitre 5 – Les systèmes du R22

## Transmission et rotor principal

Le système de transmission constitue le "cœur mécanique" du R22, reliant le moteur au rotor avec une fiabilité éprouvée.

### Architecture générale

**Composants principaux** :
- Boîte de vitesses principale (réducteur)
- Arbre de transmission rotor
- Rotor principal (2 pales)
- Système de lubrification intégré

**Ratios de transmission** :
- Rapport primaire : Moteur → Boîte = 1:1
- Rapport final : Boîte → Rotor = 9.09:1
- Régime rotor : 500 tr/min max (moteur à 2'800 tr/min)

### Boîte de vitesses principale

**Conception épicycloïdale** :
- 3 satellites planétaires
- Rapport fixe 9.09:1
- Lubrification par barbotage
- Refroidissement par convection

**Performances** :
- Rendement : 97-98%
- Capacité : 150 kW continu
- Masse : 25 kg
- Fiabilité : >10'000 heures MTBF

**Surveillance** :
- Température huile : 60-100°C
- Pression : 2.8-4.1 bar
- Vibrations : <0.5 IPS (inches/second)

### Rotor principal

**Configuration semi-rigide** :
- Deux pales en aluminium 6061-T6
- Articulations : Lead-lag et flapping uniquement
- Pas : Collectif (-10° à +27°) + Cyclique (±10°)

**Géométrie des pales** :
- Longueur : 3.835 m (bord d'attaque à extrémité)
- Corde : 19 cm (racine) à 13 cm (extrémité)
- Angle de calage : 8° (racine) à 0° (extrémité)
- Profil : NACA 23012 modifié

**Performances aérodynamiques** :
```
Surface totale : 2 × (3.835 × 0.16) = 1.23 m²
Portance maximale : ρ × A × Cl × V²/2
Cl max = 1.2 → Portance max ≈ 15'000 N
```

**Maintenance préventive** :
- Inspection visuelle : Avant chaque vol
- Contrôle de traînée : Mensuel
- Révision complète : 2'200 heures

### Rotor de queue

**Configuration coaxiale** :
- Deux pales en composite (fibre de verre)
- Diamètre : 1.42 m
- Régime : 2'240 tr/min (4.2 × rotor principal)

**Performances** :
- Poussée maximale : 1'500 N
- Puissance absorbée : 10-15 kW
- Efficacité : 65-70%

**Avantages du composite** :
- Résistance à la corrosion
- Stabilité dimensionnelle
- Réduction des vibrations

## Circuit carburant et lubrification

Les systèmes fluides assurent la lubrification et l'alimentation énergétique du R22.

### Circuit carburant

**Configuration générale** :
- Réservoir principal : 81.4 L (derrière sièges)
- Carburant : 100LL (tetraéthylplombe)
- Pompe mécanique : Injection directe
- Filtre : À l'admission carburateur

**Performances** :
- Autonomie : 3.0 heures à puissance cruise
- Consommation : 24-30 L/h
- Réserve : 30 minutes (9.1 L)

**Sécurité carburant** :
- Jauge électrique : Précision ±2 L
- Alarme réserve : 9.1 L restants
- Système anti-incendie : Soupapes coupe-feu

**Calculs opérationnels** :
```
Temps de vol disponible = (Carburant - Réserve) / Consommation
Exemple : (70 - 9.1) / 25 = 2.44 heures
```

### Système de lubrification

**Circuit fermé** :
- Carter humide : 3.8 L capacité
- Pompe à engrenages : Pression 2.8-4.1 bar
- Refroidisseur huile-air : Efficacité 80%

**Caractéristiques huile** :
- Grade : SAE 15W-50 ou équivalent
- Spécification : MIL-L-22851 ou équivalent
- Viscosité : 15 cSt à 100°C
- Additifs : Anti-usure et anti-oxydation

**Surveillance température** :
- Normale : 60-100°C
- Maximum continu : 105°C
- Alarme : 110°C (arrêt moteur recommandé)

**Maintenance** :
- Changement : 50 heures ou annuel
- Analyse : Spectrométrie (optionnel)
- Filtre : Remplacement 100 heures

## Commandes hydrauliques et électriques

Les commandes de vol utilisent des systèmes mécaniques directs, assurant fiabilité et simplicité.

### Commandes de vol mécaniques

**Cyclique** :
- Tiges push-pull : Acier haute résistance
- Course : ±10° aux pales
- Friction : Ajustable (manette rouge)
- Précession : Compensation automatique

**Collectif** :
- Câbles Bowden : Inoxydable
- Course : -10° à +27°
- Compensation RPM : Automatique
- Sécurité : Crochet anti-débrayage

**Pédales** :
- Tiges rigides : Aluminium
- Course : ±20° rotor queue
- Friction : Fixe (pas ajustable)
- Coordination : Avec collectif

### Système électrique

**Batterie principale** :
- Type : Plomb-acide 12V 25Ah
- Localisation : Derrière siège passager
- Autonomie : 30 minutes (instruments seuls)
- Charge : Alternateur 40A

**Bus électriques** :
- Bus principal : Instruments essentiels
- Bus avionique : Radio, GPS (option)
- Bus secours : Minimum pour atterrissage

**Consommation typique** :
- Instruments de base : 5-8A
- Radio + transpondeur : 2-3A
- GPS + éclairage : 1-2A
- Total croisière : 8-12A

**Protection électrique** :
- Fusibles : 5-15A selon circuits
- Disjoncteurs : Reset automatique
- Parasurtenseurs : Protection alternateur

## Instruments moteur et alarmes

Le R22 dispose d'une instrumentation moteur complète avec alarmes intégrées.

### Instruments primaires

**Tachymètre rotor** :
- Type : Magnétique (impulsion pales)
- Précision : ±1 tr/min
- Alarme : Rouge >520 tr/min

**Manifold pressure** :
- Capteur : Mécanique (membrane)
- Plage : 10-30 inHg
- Résolution : 0.5 inHg

**Température huile** :
- Sonde : Thermistance NTC
- Plage : 0-120°C
- Alarme : >110°C (voyant + buzzer)

**Pression huile** :
- Capteur : Pressostatique
- Plage : 0-7 bar
- Alarme : <2.0 bar (rouge) ou >5.5 bar (jaune)

### Alarmes et avertissements

**Système sonore** :
- Buzzer continu : RPM rotor <430 tr/min
- Buzzer intermittent : Température >110°C
- Cloche : Pression huile basse

**Voyants lumineux** :
- **Rouge** : Dangers immédiats (RPM, pression)
- **Jaune** : Conditions dégradées (température)
- **Vert** : Fonctionnement normal (alternateur)

**Logique d'alarmes** :

| Condition | Alarme | Action requise |
|-----------|--------|----------------|
| RPM <430 | Buzzer continu + voyant | Autorotation immédiate |
| Pression <2 bar | Voyant rouge | Atterrissage immédiat |
| Température >110°C | Buzzer + voyant jaune | Réduction puissance |
| Alternateur défaillant | Voyant vert OFF | Procédure secours |

### Instruments optionnels

**Heure moteur** :
- Compteur Hobbs : Temps total moteur
- Précision : 0.1 heure
- Usage : Maintenance programmée

**Tachymètre moteur** :
- Régime moteur réel
- Plage : 1'000-3'000 tr/min
- Diagnostic : Accordage carburateur

**Pyromètre** :
- Température échappement
- Détection : Richesse mélange
- Alarme : >700°C

## Maintenance et inspections

### Programme de maintenance

**Inspections quotidiennes** :
- Niveau huile : Visuel
- Carburant : Jauge + odeur
- Pales rotor : Fissures, erosion
- Commandes : Jeu excessif

**Inspections 50 heures** :
- Filtres à air : Nettoyage
- Bougies : Vérification écartement
- Batterie : Charge et électrolyte
- Transmission : Niveau huile

**Inspections 100 heures** :
- Bougies : Remplacement
- Filtres huile : Remplacement
- Câbles commandes : Tension
- Rotor : Équilibrage dynamique

### Outils de diagnostic

**Analyseur moteur** :
- Données temps réel : RPM, températures, pressions
- Enregistrement vol : Tendances et anomalies
- Maintenance prédictive : Détection prématurée

**Vibromètre** :
- Mesure vibrations : Rotor et transmission
- Seuils d'alarme : 0.5 IPS (inches/second)
- Localisation défauts : Analyse spectrale

## Synthèse du chapitre

Les systèmes du R22 témoignent d'une conception éprouvée où simplicité rime avec fiabilité. Le système mécanique direct assure une transmission de puissance efficace tandis que l'instrumentation complète permet une surveillance continue des paramètres critiques.

Cette architecture robuste explique la longévité exceptionnelle du modèle et sa popularité persistante auprès des écoles de pilotage.

---

**Évaluation** :
- Quels sont les principaux composants du système de transmission ?
- Quelle est la capacité du réservoir carburant et l'autonomie correspondante ?
- Décrivez le système d'alarmes du R22.

**Exercice de maintenance** :
Vous effectuez une inspection pré-vol. Quels éléments devez-vous vérifier en priorité ? Si la température huile indique 105°C au décollage, quelle action prenez-vous ?

**Pour aller plus loin** :
- Étudiez le manuel de maintenance Robinson R22
- Comparez avec des hélicoptères à systèmes hydrauliques
- Analysez les bulletins de service en vigueur
