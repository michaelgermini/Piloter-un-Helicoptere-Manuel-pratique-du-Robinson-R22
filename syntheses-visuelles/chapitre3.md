# Synthèse Visuelle - Chapitre 3 : Principes de vol d'un hélicoptère

## 🌪️ Forces en présence

```
PORTANCE (LIFT) ─── TRAÎNÉE (DRAG) ─── POUSSÉE (THRUST) ─── POIDS (WEIGHT)
     ↑                     ↑                ↑                    ↓
Créée rotor          Résistance      Compensation couple     Attraction terre
Perpendiculaire     Opposée mouvement  Horizontale latérale   mg = 5'886 N (600kg)
au vent relatif      au mouvement      (rotor queue)
```

## 🔄 Rotor principal et rotor de queue

```
ROTOR PRINCIPAL                 ROTOR DE QUEUE
├── Portance verticale         ├── Poussée latérale
├── Propulsion horizontale     ├── Compensation couple
├── 2 pales semi-rigides       ├── 2 pales composite
├── RPM 500 max               ├── RPM 2'240 (4.2×)
├── Pas -10° à +27°           ├── Pas ±20°
└── Puissance 93 kW           └── Puissance 10-15 kW
```

## ⚠️ Dissymétrie de portance

```
CÔTÉ AVANÇANT          CÔTÉ RECULANT
Vr = Vh + Vt            Vr = Vh - Vt
Portance ∝ Vr²          Portance ∝ Vr²

EXEMPLE (Vt=30kt, Vh=100kt):
Vr_av = 130kt → L_av = 2.45×L_moy
Vr_ar = 70kt  → L_ar = 0.49×L_moy
RATIO = 3.45:1 ⚠️ INSTABILITÉ

CORRECTION:
θ_correctif ≈ (Vt/Vh) × θ_moyen × k
Précession 90° → Commande appliquée 90° avant
```

## 🌍 Effet de sol et effet de translation

```
EFFET DE SOL                    EFFET DE TRANSLATION
├── Réduction vitesse induite  ├── Perte effet sol
├── +25% portance à h=R/2      ├── Augmentation traînée
├── Facilite décollage         ├── Baisse performance
├── Présent < 4m hauteur      ├── À partir 15kt
└── Maximum au sol            └── Progressif

GESTION:
Décollage → Profiter effet sol
Transition → Accélérer >15kt
Approche → Utiliser coussin air
```

## 📊 Équilibre dynamique

```
Σ Forces verticales = 0
Portance = Poids

Σ Forces horizontales = 0  
Poussée = Traînée

Équilibre couple:
Couple rotor = Poussée queue × Bras de levier
1'780 Nm = P_queue × 4.5 m
P_queue = 395 N
```

## 🔧 Triangle des forces rotoriques

```
VITESSE RELATIVE (Vr)
├── Composante verticale (Vi) ↓
├── Composante horizontale (Vt) →
└── Résultante Vr = √(Vt² + Vi²)

ANGLE D'ATTAQUE EFFECTIF
α_eff = arctan(Vi/Vt)

PERFORMANCE:
Vi stationnaire ≈ 3.6 m/s (600kg)
Puissance totale = P_portance + P_traînée + P_rotor_queue
```

## 📋 Évaluation chapitre

### Concepts maîtrisés
- [ ] Forces fondamentales du vol
- [ ] Fonction rotor principal/queue
- [ ] Phénomène dissymétrie
- [ ] Effets sol/translation

### Formules clés
- Portance L = ½ ρ V² S Cl
- Dissymétrie: Rapport L_av/L_ar = (Vr_av/Vr_ar)²
- Rayon virage R = V²/(g × tan θ)

### Applications pratiques
1. Compensation dissymétrie par cyclique
2. Gestion effets sol en approche
3. Calcul équilibre des forces
