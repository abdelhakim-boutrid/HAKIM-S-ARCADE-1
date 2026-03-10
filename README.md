# 🎮 Hakim's Arcade — Corp Wars FPS

## jeux developé en vibe code pour le plaisir 

## LINK : hakimarcaden1.vercel.app
<div align="center">

![Version](https://img.shields.io/badge/version-3.0-ff6a00?style=for-the-badge)
![Engine](https://img.shields.io/badge/engine-Three.js_r128-00f5ff?style=for-the-badge)
![Language](https://img.shields.io/badge/language-Vanilla_JS-ffe600?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-00ff88?style=for-the-badge)
![Size](https://img.shields.io/badge/size-Single_File-aa44ff?style=for-the-badge)

**Un FPS 3D premier personne dans votre navigateur, entièrement en Vanilla JS + Three.js**

*Survivez aux vagues interminables de l'open space techno-corporatif*

</div>

---

## 🖼️ Aperçu

> **Hakim's Arcade** est un jeu de tir à la première personne jouable directement dans un navigateur web, sans installation, sans dépendances NPM, sans build system.  
> Un seul fichier HTML. Ouvrez-le. Jouez.

Le jeu se déroule dans un open space néon dystopique où vous affrontez **12 archétypes** de collègues tech avec leurs clichés, leurs phrases, et leurs comportements caractéristiques — des stagiaires aux boss C-Level.

---

## ✨ Fonctionnalités

### 🎮 Gameplay
- **FPS 3D complet** avec moteur physique : gravité, saut (double saut), sprint
- **Grande map ouverte** (120×120 unités) avec zones de bureaux, couloirs, plateformes surélevées
- **Système de vagues** progressives (vague 1 : 6 ennemis → +3 par vague)
- **Boss Waves** toutes les 5 vagues avec avertissement dramatique
- **Système de combo kills** : enchaînez les kills pour multiplier votre score
- **Pickups au sol** : santé (+25/+50 HP), munitions (+30), XP bonus
- **Détection de collision** complète (murs, obstacles, plateformes)

### 🔫 Arme réaliste
L'arme est entièrement modélisée en 3D avec :
- Châssis (lower receiver) avec détails de rail
- Slide (upper receiver) avec cannelures de rechargement
- Canon avec couronne chromée et alésage
- Protège-détente + détente
- Crosse avec panneaux de grip
- Chargeur avec base chromée
- Hausse arrière + guidon avant avec point de mire néon
- Rail tactique + lampe tactique
- Animation de recul du slide
- Flash de bouche + lumière dynamique de tir
- Système de dispersion (spread) selon cadence de tir

### 👾 Ennemis avec personnalité
12 types d'ennemis inspirés des clichés de la tech industry :

| Ennemi | Cliché | HP | Danger |
|--------|--------|-----|--------|
| **Cyber Junior** (Stage) | *"CVE trouvée sur Wikipédia"* | 3 | ⭐ |
| **Cyber Senior** (10 ans XP) | *"Zero trust. Sauf pour moi."* | 7 | ⭐⭐ |
| **Dev Junior** (6 mois) | *"Stack Overflow c'est la doc"* | 3 | ⭐ |
| **Software Architect** (Senior) | *"Tout en microservices"* | 8 | ⭐⭐⭐ |
| **Data Junior** (Alternance) | *"Pie chart en CSS"* | 3 | ⭐ |
| **Data Scientist** (PhD) | *"P<0.05 donc c'est vrai"* | 6 | ⭐⭐ |
| **IA Évangéliste** (Influenceur) | *"GPT remplace les devs"* | 4 | ⭐⭐ |
| **CTO IA** (C-Level) | *"Stack 100% IA"* | 12 | ⭐⭐⭐⭐ |
| **RH Recruteuse** | *"5 ans XP sur React de 2 ans"* | 4 | ⭐⭐ |
| **Scrum Master** (PSM III) | *"On en parle en rétro"* | 4 | ⭐⭐ |
| **Product Manager** (VP) | *"Juste un bouton simple"* | 6 | ⭐⭐⭐ |
| **👹 PDG BOSS** | *"Mon vrai KPI c'est vous"* | 40 | ⭐⭐⭐⭐⭐ |
| **👹 CTO BOSS** | *"Je REFACTORISE TOUT"* | 30 | ⭐⭐⭐⭐⭐ |

Chaque ennemi possède :
- Un modèle 3D articulé avec torse, bras, jambes animés
- Une texture procédurale (formules mathématiques, binaire, code, neural net...)
- Un message de kill sarcastique
- Une plaque de nom flottante en billboard

### 📈 Système de carrière
Progressez à travers **12 niveaux** en accumulant de l'XP par kills :

```
Stagiaire (18k€) → Junior Dev (32k€) → Développeur (42k€) → Dev Confirmé (52k€)
→ Senior Dev (65k€) → Tech Lead (78k€) → Staff Engineer (90k€)
→ Principal Eng. (105k€) → Architect (120k€) → Eng. Manager (140k€)
→ VP Engineering (165k€) → CTO (200k€/an) 🏆
```

### 🗺️ Interface & HUD
- **Mini-map temps réel** (coin bas-droit) avec ennemis, pickups, direction du joueur
- **Barres de santé et XP** animées
- **Kill feed** avec noms, messages et scores
- **Name tag** sur l'ennemi dans la ligne de mire (rôle, nom, barre de vie)
- **Compteur de combo** animé (×3, ×4, ×5...)
- **Viseur dynamique** avec indicateur de dispersion
- **HUD carrière** : titre, niveau, salaire, score, vague

### 🌧️ Visuels & Effets
- Rendu **ACESFilmic** tone mapping
- **Pluie néon** verticale (200 particules cyan)
- **Étincelles** à l'impact des balles (système de pool)
- **4 lumières néon** pulsantes (orange, cyan, violet, vert)
- Flash de **vignette rouge** quand touché
- Flash **vert** quand un pickup est ramassé
- Piliers néon lumineux aléatoires
- Grille au plafond multicolore

---

## 🕹️ Contrôles

| Touche | Action |
|--------|--------|
| `W` / `Z` / `↑` | Avancer |
| `S` / `↓` | Reculer |
| `A` / `Q` / `←` | Gauche |
| `D` / `→` | Droite |
| `ESPACE` | Sauter (double saut disponible) |
| `SHIFT` | Sprint |
| `Clic gauche` | Tirer |
| `R` | Recharger |
| `ESC` | Libérer la souris / pause |

> **Note** : Le jeu capture la souris au clic. Cliquez sur le canvas pour reprendre après une pause.

---

## 🚀 Installation & Utilisation

### Option 1 — Ouvrir directement
```bash
# Téléchargez hakims-arcade.html
# Double-clic → ouvre dans votre navigateur
```

### Option 2 — Serveur local (recommandé pour les perfs)
```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```
Puis ouvrez `http://localhost:8000/hakims-arcade.html`

### Option 3 — GitHub Pages
1. Forkez ce repo
2. Activez GitHub Pages (Settings → Pages → Source: main branch)
3. Accédez à `https://votre-username.github.io/hakims-arcade/hakims-arcade.html`

---

## 🔧 Stack technique

```
hakims-arcade.html          ← tout est ici, ~1200 lignes
│
├── Three.js r128            ← moteur 3D (CDN)
│   ├── WebGLRenderer        ← ACESFilmic tone mapping
│   ├── PerspectiveCamera    ← FOV 76°, near 0.05
│   ├── Scene + Fog          ← FogExp2 pour l'ambiance
│   ├── DirectionalLight     ← shadow map 4096×4096
│   └── PointLights          ← lumières néon dynamiques
│
├── Physique custom          ← gravité, saut, collision AABB
├── Canvas 2D                ← textures procédurales + minimap
└── Vanilla JS               ← zéro framework, zéro NPM
```

**Aucune dépendance** autre que Three.js chargé via CDN.  
**Aucun build** requis. Modifiez le HTML, rechargez, jouez.

---

## 📊 Architecture du code

```
CAREER[]         → 12 niveaux de carrière avec seuils XP
TYPES[]          → 13 types d'ennemis (12 normaux + boss)

makeEnemyTex()   → génère les textures procédurales par skin type
spawnEnemy()     → instancie un ennemi avec modèle 3D articulé
spawnPickup()    → crée un item au sol (santé, ammo, XP)

Physics engine:
  getGroundY()   → hauteur du sol / plateformes sous le joueur
  resolveCol()   → résolution AABB pour joueur et ennemis
  GRAVITY=22     → accélération gravitationnelle
  JUMP_VEL=9.5   → vitesse initiale du saut

Weapon:
  shoot()        → tire une balle avec dispersion + recul
  slideKick      → animation du slide au tir
  spreadAmount   → augmente à la cadence, réduit au repos

Rendering:
  animate()      → game loop principale (~60 fps)
  drawMinimap()  → minimap canvas 2D 130×130px
  updateSparks() → pool de 60 particules d'étincelles
  updateRain()   → 200 points de pluie néon
```

---

## 🎯 Roadmap / Idées d'améliorations

- [ ] Plusieurs armes (shotgun, SMG, sniper)
- [ ] Ennemis avec pathfinding (A*)
- [ ] Mode multijoueur (WebSocket)
- [ ] Système de save (localStorage)
- [ ] Achievements / trophées
- [ ] Sons et musique (Web Audio API)
- [ ] Ombres dynamiques améliorées (PCSShadowMap)
- [ ] Post-processing (bloom, chromatic aberration)
- [ ] Map procédurale générée à chaque partie
- [ ] Mode "Survie infinie" vs mode "Campagne"

---

## 📸 Screenshots

> *(À venir — ouvrez le jeu et faites F12 → Console → `renderer.domElement.toDataURL()` pour capturer)*

---

## 🤝 Contribution

Les contributions sont les bienvenues !

```bash
git clone https://github.com/votre-username/hakims-arcade.git
cd hakims-arcade
# Modifiez hakims-arcade.html
# Ouvrez dans le navigateur pour tester
```

Suggestions bienvenues :
- Nouveaux types d'ennemis (avec leur cliché)
- Nouveaux messages de kill sarcastiques
- Améliorations de gameplay
- Corrections de bugs physique

---

## 📄 Licence

MIT — Faites-en ce que vous voulez.

```
Copyright (c) 2025 Hakim's Arcade
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software...
```

---

<div align="center">

**Fait avec ❤️ et beaucoup trop de réunions Zoom**

*"Works on my machine"* — DevOps Guru, vague 3

</div>
