# Chapitre 3 – Principes de vol d'un hélicoptère

## Forces en présence : portance, traînée, poussée

Le vol d'un hélicoptère repose sur l'équilibre délicat de quatre forces fondamentales, similaire à l'avion mais avec des particularités uniques dues au rotor.

### Les quatre forces du vol

**1. Portance (Lift)** : Force verticale créée par le rotor
- Direction : Vers le haut, perpendiculaire au vent relatif
- Origine : Pression différentielle sur les pales
- Contrôle : Via le pas collectif et cyclique

**2. Traînée (Drag)** : Résistance à l'avancement
- Direction : Oppposée au mouvement
- Composantes : Profil + induite
- Impact : Réduction de la performance

**3. Poussée (Thrust)** : Force propulsive du rotor de queue
- Direction : Horizontale, latérale
- Origine : Réaction du rotor de queue
- Fonction : Compensation du couple moteur

**4. Poids (Weight)** : Attraction terrestre
- Direction : Vers le bas
- Valeur : Masse × accélération gravitationnelle
- Constante : 9.81 m/s²

### Équilibre dynamique

En vol stationnaire, l'équilibre s'exprime par :

```
∑ Forces verticales = 0 : Portance = Poids
∑ Forces horizontales = 0 : Poussée = Traînée
```

**Exemple numérique** :
Pour un R22 en stationnaire (masse 600 kg) :
- Poids = 600 × 9.81 = 5'886 N
- Portance requise = 5'886 N
- Puissance nécessaire ≈ 30 kW (40 ch)

### Triangle des forces rotoriques

Le rotor crée simultanément portance et propulsion :

```
Vitesse induite (Vi) : Composante verticale descendante
Vitesse de translation (Vt) : Composante horizontale
Vitesse relative (Vr) : Résultante = Vt + Vi
```

**Calcul de la vitesse relative** :
```
Vr = √(Vt² + Vi²)
Angle d'attaque effectif = arctan(Vi/Vt)
```

## Rotor principal et rotor de queue

Le système rotorique du R22 fonctionne selon le principe de l'autorotation contrôlée, où deux rotors complémentaires assurent la stabilité et le contrôle.

### Rotor principal : cœur du système

**Configuration semi-rigide** :
- Deux pales en aluminium nervurées
- Articulation : Flapping et lead-lag uniquement
- Pas variable : Collectif (-10° à +27°) + Cyclique (±10°)

**Aérodynamique des pales** :
- Profil NACA 23012 modifié
- Cordé : 19 cm à la racine, 13 cm à l'extrémité
- Angle de calage : Progression linéaire de 8° à 0°

**Performances calculées** :
```
Portance maximale par pale : ρ × A × Cl × V²/2
A = Surface de la pale = Longueur × Cordé moyenne
Cl = Coefficient de portance (max 1.2)
```

### Rotor de queue : stabilisateur directionnel

**Configuration coaxiale** :
- Deux pales en composite (fibre de verre)
- Régime : 4.2 × régime rotor principal (2'100 tr/min)
- Puissance absorbée : 10-15% de la puissance totale

**Principe de fonctionnement** :
- Le rotor principal crée un couple antihoraire
- Le rotor de queue compense par une poussée horaire
- Équilibre : Couple rotor = Poussée queue × Distance

**Calcul du couple** :
```
Couple moteur = Puissance / (2π × Régime)
Couple rotor = Couple moteur × (1 - Rendement transmission)
Poussée queue = Couple rotor / Bras de levier
```

**Exemple R22** :
- Puissance moteur : 93 kW
- Rendement transmission : 95%
- Couple rotor : 1'780 Nm
- Poussée queue : 1'100 N (en croisière)

## Dissymétrie de portance

La dissymétrie de portance représente le défi aérodynamique majeur du rotor en translation. Sans correction, elle causerait une perte de contrôle catastrophique.

### Origine physique

**Phénomène fondamental** :
- Côté avançant : Vitesse relative = Vhélice + Vtranslation
- Côté recul : Vitesse relative = Vhélice - Vtranslation

**Conséquence** :
```
Portance côté avançant ∝ (Vh + Vt)²
Portance côté recul ∝ (Vh - Vt)²
ΔPortance = Portance_avant - Portance_arrière
```

**Exemple numérique** (Vtranslation = 30 kt, Vhélice = 100 kt) :
- Côté avançant : Vr = 130 kt → Portance × 1.69
- Côté recul : Vr = 70 kt → Portance × 0.49
- Rapport : 3.45:1 ⚠️ **Instabilité majeure**

### Compensation par le cyclique

**Principe de correction** :
- Réduire le pas côté avançant (portance excessive)
- Augmenter le pas côté recul (portance insuffisante)

**Angle de correction** :
```
θ_correctif ≈ (Vt / Vh) × θ_pas_moyen
Pour Vt = 30 kt, Vh = 100 kt : θ ≈ 6-8°
```

**Effet gyroscopique** :
- Précession de 90° dans le sens de rotation
- Commande appliquée 90° avant la pale concernée

### Limites de la compensation

**Vitesse maximale de translation** :
- Dissymétrie devient incompressible
- Angle de correction maximal atteint (±10° cyclique)
- Vne = 190 km/h pour le R22

## Effet de sol et effet de translation

Deux phénomènes aérodynamiques modifient significativement les performances près du sol.

### Effet de sol (Ground Effect)

**Principe physique** :
- Le sol empêche l'accélération descendante de l'air
- Réduction de la vitesse induite (Vi diminue de 20-30%)
- Augmentation de la portance pour même puissance

**Zone d'influence** :
- Hauteur efficace : Rayon rotor / 2 (≈ 4 m pour R22)
- Maximum à h = 0.5 × Rayon rotor

**Calcul de l'effet** :
```
Portance avec effet = Portance sans effet × (1 + (Rayon_rotor / (4 × h))²)
À h = Rayon_rotor/2 : Augmentation ≈ 25%
```

**Avantages opérationnels** :
- Puissance requise réduite pour le décollage
- Manoeuvre plus douce en approche

### Effet de translation

**Transition sol-air** :
- Perte progressive de l'effet de sol
- Augmentation de la traînée induite
- Baisse de performance transitoire

**Phénomène inverse en descente** :
- Air comprimé sous le rotor
- "Coussin d'air" facilitant l'approche
- Risque de flottement (flaring)

**Gestion pratique** :
- Décollage : Profiter de l'effet de sol initial
- Transition : Accélérer progressivement (> 15 kt)
- Approche : Utiliser l'effet pour l'arrondi

## Synthèse du chapitre

Les principes de vol hélicoptère reposent sur des phénomènes aérodynamiques complexes où chaque force interagit avec les autres. La dissymétrie de portance, défi majeur du rotor en translation, est maîtrisée par le cyclique tandis que les effets de sol et de translation influencent les manoeuvres près du terrain.

Comprendre ces principes permet d'anticiper les réactions de l'appareil et d'optimiser les performances.

---

**Évaluation** :
- Quelles sont les quatre forces fondamentales du vol ?
- Expliquez le phénomène de dissymétrie de portance.
- Quelle est la différence entre effet de sol et effet de translation ?

**Exercice de calcul** :
Pour un R22 en vol stationnaire (masse 600 kg), calculez la portance minimale requise. Sachant que la surface rotor est de 46 m² et que le coefficient de portance maximal est de 1.1, quelle vitesse induite minimale est nécessaire ?

**Pour aller plus loin** :
- Étudiez les équations de la portance rotorique
- Observez un rotor en mouvement lent
- Comparez avec l'aérodynamique des voilures fixes
