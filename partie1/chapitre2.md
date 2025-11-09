# Chapitre 2 – Présentation du Robinson R22

## Histoire et caractéristiques techniques

Le Robinson R22 est bien plus qu'un simple hélicoptère d'école. Né de l'ambition d'un homme visionnaire, Frank Robinson, il incarne la démocratisation du vol rotorique léger.

### Genèse du projet (1973-1975)

Frank Robinson, ancien pilote d'essai chez Bell Helicopter, identifie un marché inexploité : l'hélicoptère d'entraînement abordable. Son analyse révèle que :

- Le marché des hélicoptères légers stagne depuis les années 60
- Les appareils d'école existants sont soit trop complexes, soit trop coûteux
- Une demande croissante existe pour la formation civile

> 💡 **Vision entrepreneuriale**
> "Je voulais créer un hélicoptère aussi simple à piloter qu'une voiture, mais capable de voler partout." - Frank Robinson

### Développement et certification

**Phase de conception (1973-1974)** :
- Études aérodynamiques avec l'Université de Stanford
- Tests en soufflerie pour optimiser l'efficacité rotorique
- Choix du moteur Lycoming O-235 pour sa fiabilité

**Prototypes et essais (1974-1975)** :
- Premier vol du prototype N21487 le 28 août 1975
- 1'200 heures d'essais en vol accumulées
- Certification FAA obtenue le 22 mars 1979

**Évolution du modèle** :
- **R22 (1979)** : Version de base avec moteur 115 ch
- **R22 Alpha (1985)** : Améliorations structurelles
- **R22 Beta (1989)** : Refonte majeure avec moteur 131 ch
- **R22 Beta II (2000)** : Modernisation avionique et sécurité

### Données techniques essentielles

| Caractéristique | Valeur | Unité |
|----------------|--------|-------|
| **Longueur** | 8.76 | m |
| **Hauteur** | 2.72 | m |
| **Diamètre rotor** | 7.67 | m |
| **Masse à vide** | 366 | kg |
| **Masse maximale** | 635 | kg |
| **Charge utile maximale** | 269 | kg |
| **Vitesse de croisière** | 170 | km/h |
| **Vitesse maximale** | 190 | km/h |
| **Plafond pratique** | 4'270 | m |
| **Autonomie** | 3.0 | heures |

## Le moteur Lycoming et le système rotor

Le cœur mécanique du R22 repose sur deux systèmes complémentaires : le moteur et le rotor principal.

### Le moteur Lycoming O-235-N2C

**Architecture générale** :
- Moteur à 4 cylindres à plat, refroidi par air
- Alésage × course : 111 mm × 98 mm
- Cylindrée : 3'802 cm³
- Puissance maximale : 124 ch (93 kW) à 2'800 tr/min

**Caractéristiques opérationnelles** :
- **Consommation spécifique** : 0.32 kg/ch/h
- **Régime de croisière** : 2'400 tr/min
- **Température d'huile normale** : 60-100°C
- **Pression d'huile** : 2.8-4.1 bar

> ⚠️ **Point critique** : Le moteur Lycoming est sensible au surcroît. Un régime supérieur à 2'800 tr/min peut causer des dommages irréversibles.

**Système d'injection** :
- Carburateur Marvel-Schebler MA4-5
- Pompe d'injection mécanique
- Enrichisseur automatique pour le décollage

### Le système rotor principal

**Configuration semi-rigide à deux pales** :
- Matériau : Aluminium 6061-T6
- Profil aérodynamique : NACA 23012 modifié
- Pas collectif : -10° à +27°
- Pas cyclique : ±10°

**Transmission et boîte de vitesses** :
- Réducteur principal : Rapport 9.09:1
- Régime rotor : 500 tr/min maximum
- Lubrification : Carter sec avec pompe
- Capacité huile : 3.8 litres

**Rotor de queue** :
- Deux pales en composite
- Diamètre : 1.42 m
- Régime : 2'240 tr/min (4.2 × régime principal)
- Fonction : Contre-rotation du couple moteur

## Poids, centrage et limites d'exploitation

La sécurité du R22 dépend directement du respect des limites de poids et centrage. Ces paramètres influencent directement les performances et la stabilité.

### Limites de poids

**Masses opérationnelles** :
- **Masse à vide typique** : 408 kg (avec équipements standard)
- **Masse maximale au décollage** : 635 kg
- **Masse maximale à l'atterrissage** : 635 kg

**Calcul de la charge utile** :
```
Charge utile = Masse maximale - Masse à vide - Carburant - Huile
```

**Exemple pratique** :
- Masse à vide : 408 kg
- Carburant plein (81.4 L × 0.72 kg/L) : 58.6 kg
- Huile : 3.5 kg
- Pilote + passager : 170 kg
- Bagages : 20 kg

*Charge utile disponible : 635 - (408 + 58.6 + 3.5) = 164.9 kg*
*Charge embarquée : 170 + 20 = 190 kg → **SURCHARGE** ❌*

### Cadrage et stabilité

Le centrage du R22 s'exprime en pourcentage de la corde moyenne aérodynamique :

**Limites de centrage** :
- Avant : 89.5 cm du pivot rotor
- Arrière : 107.2 cm du pivot rotor
- Fourchette acceptable : 95.5% - 106.2% MAC (Mean Aerodynamic Chord)

**Calcul du centrage** :
```
Centrage (%) = [(Moment total) / (Masse totale × Longueur MAC)] × 100
```

**Tableau des bras de levier** :

| Élément | Bras de levier (cm) | Position par rapport au pivot |
|---------|-------------------|-------------------------------|
| Siège pilote | 89.5 | Avant |
| Siège passager | 107.2 | Arrière |
| Réservoir principal | 97.8 | Central |
| Bagages arrière | 132.1 | Arrière |

### Limites environnementales

**Conditions de température** :
- **Minimale** : -20°C (avec préchauffage)
- **Maximale** : +50°C
- **Densité altitude** : Correction automatique requise

**Limites de vent** :
- **Décollage/atterrissage** : 24 nœuds maximum
- **Vol en croisière** : 65 nœuds maximum
- **Vent de travers** : 17 nœuds maximum

**Conditions météorologiques** :
- **Visibilité minimale** : 1.5 km (VFR de jour)
- **Plafond minimal** : 300 m AGL
- **Turbulence** : Éviter catégories modérée à sévère

## Évolution et modernisations

Le R22 continue d'évoluer pour rester au sommet de sa catégorie :

### Améliorations structurelles
- **Renforts fuselage** : Résistance aux vibrations accrues
- **Sièges ergonomiques** : Confort et sécurité améliorés
- **Portes coulissantes** : Accès facilité

### Avionique moderne (R22 Beta II)
- **GPS intégré** : Navigation précise
- **Transpondeur Mode S** : Identification automatique
- **Système audio** : Communications claires
- **Instruments numériques** : Lecture facilitée

### Sécurité renforcée
- **Siège crash-resistant** : Protection impact
- **Harnais à inertie** : Réduction des blessures
- **Systèmes d'alarme** : Alertes précoces

## Synthèse du chapitre

Le Robinson R22 représente l'équilibre parfait entre simplicité, fiabilité et performances. Sa conception épurée cache une sophistication technique remarquable, fruit de décennies d'expérience et d'améliorations continues.

Comprendre ses caractéristiques fondamentales - moteur, rotor, limites de poids - est essentiel pour exploiter pleinement ses capacités tout en préservant la sécurité.

---

**Évaluation** :
- Pouvez-vous citer les principales limites de poids du R22 ?
- Quelle est la fonction du rotor de queue ?
- Comment calcule-t-on le centrage d'un hélicoptère ?

**Exercice pratique** :
Calculez la charge utile disponible pour un R22 dont la masse à vide est de 410 kg, avec 70 litres de carburant et tous les fluides.

**Pour aller plus loin** :
- Consultez le manuel de vol Robinson R22
- Étudiez les bulletins de service applicables
- Comparez avec d'autres hélicoptères d'école (R44, Schweizer 300)
