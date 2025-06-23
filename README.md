# 💰 Calculateur TJM - "Calculez votre Taux Journalier Moyen en tant que freelance"

**Calculateur TJM** est une application web moderne développée avec **Vue.js** et **Tailwind CSS**. Elle permet aux freelances et consultants de calculer précisément leur **Taux Journalier Moyen (TJM)** en prenant en compte tous les paramètres essentiels :

- 💸 Salaire net souhaité
- 🏢 Frais de fonctionnement détaillés
- 📊 Charges sociales (micro-entreprise, EURL, SASU...)
- 🧾 Impositions et versement libératoire
- 📅 Décompte des jours travaillés et non facturables
- 📈 Marge bénéficiaire

## 🚀 Site en ligne

> https://calculateur-de-tjm.netlify.app

---

## ✨ Fonctionnalités

### 🎯 Calcul intelligent du TJM
- **Slider interactif** pour définir le salaire net mensuel souhaité
- **Calcul automatique** du chiffre d'affaires annuel nécessaire
- **Estimation précise** du taux journalier moyen

### 💼 Gestion complète des frais
- **12 catégories de frais** : loyer, déplacements, logiciels, comptabilité...
- **Interface collapse/expand** pour une meilleure organisation
- **Calcul automatique** des totaux mensuels et annuels

### 📊 Charges sociales et fiscalité
- **Support multi-statuts** : micro-entreprise, EURL, SASU
- **Toggle mensuel/annuel** pour l'affichage des charges
- **Versement libératoire** pris en compte
- **Taux d'imposition personnalisable**

### 📅 Décompte des jours
- **Jours ouvrés** calculés automatiquement (251 jours/an)
- **Jours non facturables** : congés, maladie, prospection, administratif
- **Marge bénéficiaire** configurable (5% à 30%)

### 📸 Export et sauvegarde
- **Export PNG** haute qualité de la simulation
- **Capture intelligente** avec padding et contraste optimisé
- **Support mode sombre** avec conversion automatique des couleurs

---

## 🛠️ Stack technique

- **Vue.js 3** (Composition API) avec système de composants modulaires
- **Vue Router** pour la navigation
- **Tailwind CSS** pour un design moderne et responsive
- **html2canvas** pour la capture d'écran PNG
- **Vite** pour un développement rapide
- **Composables Vue** pour la logique métier réutilisable

### 🏗️ Architecture

```
src/
├── components/
│   ├── Landing/           # Composants de la landing page
│   └── Calculateur/       # Composants du calculateur
│       ├── Remuneration.vue
│       ├── FraisFonctionnement.vue
│       ├── ChargesSociales.vue
│       ├── Impositions.vue
│       ├── DecompteJour.vue
│       └── EstimationFinale.vue
├── composables/
│   └── useCalculator.js   # Logique métier du calculateur
├── pages/                 # Pages de l'application
└── router.js             # Configuration des routes
```

---

## 📦 Installation et développement

```bash
# Clone du dépôt
git clone https://github.com/votre-username/TJMCalculator.git
cd TJMCalculator

# Installation des dépendances
npm install

# Lancement du serveur de développement
npm run dev

# Build pour la production
npm run build

# Prévisualisation du build
npm run preview
```

## 🎨 Fonctionnalités techniques avancées

### ⚡ Réactivité optimisée
- **Computed properties** pour des calculs performants
- **Système inject/provide** pour le partage d'état
- **Gestion fine des événements** avec `:value` et `@input`

### 🎭 Interface adaptative
- **Mode sombre/clair** automatique
- **Design responsive** mobile-first
- **Animations CSS** fluides pour les interactions

### 📱 Export intelligent
- **Détection automatique** du mode sombre
- **Conversion des couleurs** pour un contraste optimal
- **Padding automatique** et qualité haute résolution

---

## 🚀 Déploiement

L'application est optimisée pour un déploiement sur :
- **Netlify** (recommandé)
- **Vercel**
- **GitHub Pages**
- Tout hébergeur supportant les SPA

---

## 📄 Licence

MIT © [jeremien6 - contact@jeremiecode.fr]

---

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- 🐛 Signaler des bugs
- 💡 Proposer des améliorations
- 🔧 Soumettre des pull requests

---

## 📞 Support

Pour toute question ou suggestion :
- 📧 Email : contact@jeremiecode.fr
- 🌐 Site : https://calculateur-de-tjm.netlify.app