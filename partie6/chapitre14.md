# Chapitre 14 – Aérodynamique avancée

## Dissymétrie de portance détaillée

La dissymétrie de portance représente le défi aérodynamique majeur du rotor en translation, nécessitant une compréhension approfondie pour une maîtrise parfaite.

### Analyse mathématique

**Phénomène fondamental** :
Considérons un rotor avançant à vitesse V_translation. Chaque pale parcourt un cercle à vitesse angulaire Ω.

La vitesse relative de chaque pale varie selon sa position :
- **Côté avançant** : Vr_av = Ωr + V_translation
- **Côté recul** : Vr_ar = Ωr - V_translation

**Angle d'attaque local** :
```
α_local = α_pas + arctan(Vi / Vr)
```

Où Vi est la vitesse induite descendante.

**Portance différentielle** :
```
ΔL = (1/2)ρ Cl S (Vr_av² - Vr_ar²)
```

Pour V_translation = 0.3 × Ωr (cas typique) :
- Vr_av = 1.3 × Ωr → L_av = 1.69 × L_moyenne
- Vr_ar = 0.7 × Ωr → L_ar = 0.49 × L_moyenne

**Résultat** : Rapport portance 3.45:1 ⚠️ Instabilité majeure

### Compensation par le cyclique

**Principe de correction** :
Le cyclique applique un pas différentiel θ_cyclique pour compenser la dissymétrie.

**Angle de correction requis** :
```
θ_correctif ≈ (V_translation / Ωr) × θ_pas_moyen × k
```

Où k ≈ 0.8-1.0 selon la conception rotor.

**Effet de précession gyroscopique** :
- La commande cyclique doit être appliquée 90° avant la pale concernée
- Le rotor "précesse" comme un gyroscope
- Délai réponse ≈ 90°/(Ω/2π) ≈ 0.09 seconde

### Limites de compensation

**Course cyclique maximale** :
- R22 : ±10° de pas cyclique
- Limite atteinte à V_translation ≈ 35-40 m/s (135 kt)
- Vno = 190 km/h (limite structurelle)

**Au-delà de la limite** :
- Vibrations accrues
- Perte de contrôle possible
- Conception rotor optimisée nécessaire

### Facteurs influençant

**Vitesse de translation** :
- Linéaire avec V_translation jusqu'à 0.4 × Ωr
- Non-linéaire au-delà (compression des extrémités)

**Vitesse induite** :
- Vi diminue en translation (moins de portance requise)
- Effet bénéfique sur la dissymétrie

**Angle de pas collectif** :
- Influence l'amplitude de la dissymétrie
- Plus de pas = dissymétrie plus marquée

## Effet gyroscopique et précession

Le rotor principal constitue un gyroscope massif soumis à des forces complexes.

### Gyroscopie fondamentale

**Moment angulaire** :
```
H = I × Ω
```

Où I est le moment d'inertie du rotor, Ω la vitesse angulaire.

Pour le R22 :
- I ≈ 15-20 kg⋅m² (estimation)
- Ω = 500 tr/min = 52.36 rad/s
- H ≈ 785-1'047 N⋅m⋅s

**Précession** :
Toute force appliquée sur le gyroscope produit un mouvement perpendiculaire à 90° dans le sens de rotation.

**Application rotor** :
- Force verticale (portance) → mouvement latéral
- Force latérale (cyclique) → mouvement vertical
- Délai 90° de phase

### Précession en action

**Commande cyclique avant** :
- Appliquée côté gauche rotor
- Produit mouvement vers le bas
- Résultat : tangage positif (montée)

**Commande cyclique droite** :
- Appliquée côté arrière rotor
- Produit mouvement vers la gauche
- Résultat : roulis droit

### Effets secondaires

**Flapping** :
- Les pales se déforment sous l'effet des forces
- Compensation automatique de la dissymétrie
- Réduction des contraintes mécaniques

**Lead-lag** :
- Mouvement longitudinal des pales
- Absorption des variations de vitesse
- Stabilité améliorée

### Applications pratiques

**Manoeuvres dynamiques** :
- Précession explique les réponses retardées
- Anticipation nécessaire des commandes
- Coordination temporelle essentielle

**Stabilité** :
- Gyroscopie maintient l'orientation
- Résistance aux perturbations
- Amortissement des oscillations

## Couple moteur et compensation

Le couple moteur représente la force de rotation que doit compenser le rotor de queue.

### Origine du couple

**Principe physique** :
La poussée rotor crée un couple opposé au moteur :
```
Couple_rotor = Puissance_moteur / Ω_rotor
```

**Calcul R22** :
- Puissance max : 93 kW
- Ω_rotor : 52.36 rad/s
- Couple : 1'780 N⋅m

**Direction** : Anti-horaire (vue de dessus)

### Compensation rotor queue

**Principe** :
Le rotor de queue produit une poussée horizontale :
```
Poussée_queue = Couple_rotor / Bras_levier
```

**Paramètres R22** :
- Bras de levier : ≈ 4.5 m
- Poussée max : ≈ 395 N
- Régime rotor queue : 4.2 × rotor principal

### Variations dynamiques

**Influence collectif** :
- Collectif ↑ → Puissance ↑ → Couple ↑ → Poussée_queue ↑
- Coordination nécessaire : pédales avec collectif

**Influence vitesse** :
- Haute vitesse : Effet vent relatif réduit le couple
- Basse vitesse : Couple plus marqué
- Transition critique : Gestion pédales fine

### Gestion pratique

**Coordination optimale** :
1. Mouvement collectif
2. Ajustement gaz pour RPM
3. Correction pédales progressive
4. Stabilisation finale

**Erreurs courantes** :
- Pédales insuffisantes → rotation appareil
- Pédales excessives → fatigue musculaire
- Coordination retardée → oscillations

## Forces inertielles et G

Les forces d'inertie jouent un rôle crucial dans les manoeuvres dynamiques.

### Accélération et G

**Charge G verticale** :
```
nz = L / (m × g) = (ρ V² S Cl) / (2 m g)
```

**Limites physiologiques** :
- nz_max = +2.0 G (R22 en virage serré)
- nz_min = -0.5 G (décélérations)

### Effets sur le pilote

**G positif (>1)** :
- Sang drainé vers pieds
- Vision grise/noire possible
- Respiration difficile

**G négatif (<1)** :
- Sang vers tête
- Vision rouge
- Désorientation

### Gestion des G

**Techniques anti-G** :
- Respiration : Expiration forcée
- Muscles : Contraction abdomen
- Vision : Concentration point fixe

**Limites R22** :
- Virage standard : +1.2 à +1.5 G
- Manoeuvres dynamiques : +2.0 G max
- Structure : Certifiée +2.5 G

## Aérodynamique rotor avancée

### Théorie de l'élément de pale

**Portance locale** :
Chaque élément de pale obéit :
```
dL = (1/2) ρ Cl(r) Vr(r)² c dr
```

**Intégration le long de la pale** :
```
L_pale = ∫ (1/2) ρ Cl(r) Vr(r)² c dr
```

### Facteur de solidité

**Définition** :
```
σ = (Nb × c × R) / (π R²) = 3 Nb c / π R
```

**R22** :
- Nb = 2 pales
- c = 0.16 m (moyen)
- R = 3.835 m
- σ ≈ 0.08 (faible pour stabilité)

### Nombre d'Avance

**Avance globale** :
```
μ = V_translation / (Ω R)
```

**Régime** :
- Stationnaire : μ = 0
- Croisière : μ = 0.3-0.35
- Maximum : μ = 0.4 (limite dissymétrie)

### Rendement rotorique

**Figure de mérite** :
```
M = Puissance_idéale / Puissance_fournie
```

**Facteurs influençant** :
- Profil aérodynamique
- Nombre de pales
- Vitesse de pointe
- Conditions atmosphériques

**R22 typique** :
- M = 0.65-0.75 en croisière
- Maximum en stationnaire : M ≈ 0.8

## Applications mathématiques

### Calculs de performance

**Vitesse induite stationnaire** :
```
Vi = √(m g / (2 ρ A))
```

R22 stationnaire :
- m = 600 kg
- A = π (3.835)² ≈ 46 m²
- ρ = 1.225 kg/m³
- Vi ≈ 3.6 m/s

**Puissance requise** :
```
P = m g Vi + P_profil + P_parasite
P_profil = pertes aérodynamiques
P_parasite = traînée fuselage
```

### Optimisation de vol

**Vitesse économique** :
Minimisation consommation :
```
C = P / V_tas
```

Où P = puissance, V_tas = vitesse vraie.

**Résultat** : V_econ ≈ 80-100 kt pour le R22.

### Analyse de manoeuvres

**Rayon de virage** :
```
R = V² / (g tan φ)
```

Avec φ = angle d'inclinaison.

**Temps de virage** :
```
t = (2π R) / V = 2π V / (g tan φ)
```

## Synthèse du chapitre

L'aérodynamique avancée révèle la complexité fascinante du vol rotorique. Des équations de dissymétrie aux calculs de performance, chaque phénomène physique trouve son application pratique dans la maîtrise du R22.

Cette compréhension approfondie transforme l'empirisme en science, permettant une anticipation précise des réactions de l'appareil.

---

**Évaluation** :
- Expliquez mathématiquement la dissymétrie de portance.
- Quel est le rôle de la précession gyroscopique dans le pilotage ?
- Comment calculez-vous le couple moteur d'un hélicoptère ?

**Exercice de calcul** :
Pour un R22 en translation à 100 kt (51.4 m/s), calculez le rapport de portance entre côté avançant et recul. Ω = 52 rad/s, R = 3.8 m.

**Pour aller plus loin** :
- Étudier les équations de McCormick pour rotors
- Analyser les données de vol du R22
- Comparer avec d'autres systèmes rotoriques
