# Tickethack Frontend

Une application web pour la réservation de billets de train, développée en collaboration avec Nicolas Portier.

**Projet d'apprentissage réalisé dans le cadre de ma formation à La Capsule.**

## 🚀 Fonctionnalités

- **Recherche de trajets** : Formulaire de recherche avec ville de départ, d'arrivée et date
- **Gestion du panier** : Ajout et suppression des trajets, calcul du total
- **Réservations** : Consultation des trajets réservés
- **Interface responsive** : Design adaptatif

## 📁 Structure du projet

```
tickethack-frontend/
├── index.html          # Page d'accueil et recherche
├── cart.html           # Page du panier
├── bookings.html       # Page des réservations
├── style.css           # Styles pour la page d'accueil
├── cart.css            # Styles pour le panier et les réservations
├── bookings.css        # Styles spécifiques aux réservations
├── script.js           # Logique de la page d'accueil
├── cart.js             # Logique du panier
├── bookings.js         # Logique des réservations
└── images/             # Ressources images
```

## 🛠️ Technologies utilisées

- **HTML5** : Structure des pages
- **CSS3** : Styles avec Flexbox
- **JavaScript** : Logique côté client avec fetch API
- **Google Fonts** : Police Roboto

## 🎨 Design

- **Palette de couleurs** : Vert nature (#4ea891) et tons neutres
- **Typographie** : Google Fonts Roboto
- **Layout** : Design centré avec cartes et éléments arrondis
- **UX** : Interface intuitive avec feedback visuel

## 🚦 Installation et utilisation

### Prérequis
- Un serveur web local (Live Server, http-server, etc.)
- Navigateur moderne

### Installation

```bash
# Cloner le repository
git clone [url-du-repo]
cd tickethack-frontend

# Lancer un serveur local
npx http-server .
# Ou utiliser Live Server dans VS Code
```

### Configuration
Pour le développement local, modifier l'URL du backend dans les fichiers JavaScript :

```javascript
// Dans script.js, cart.js, bookings.js
const MYURL = 'http://localhost:3000';
```

## 📱 Pages de l'application

### Page d'accueil (index.html)
- Formulaire de recherche de trajets (départ, arrivée, date)
- Affichage des résultats de recherche
- Bouton "Book" pour ajouter au panier

### Page panier (cart.html)
- Liste des trajets dans le panier
- Bouton de suppression (X) pour chaque trajet
- Calcul automatique du total
- Bouton "Purchase" pour finaliser

### Page réservations (bookings.html)
- Affichage des trajets réservés
- Informations sur le temps restant avant le départ

## 🔄 Flux utilisateur

1. **Recherche** : L'utilisateur saisit ses critères de voyage
2. **Sélection** : Les trajets disponibles s'affichent avec option de réservation
3. **Panier** : Les trajets sélectionnés sont ajoutés au panier
4. **Achat** : Confirmation et finalisation de la commande
5. **Suivi** : Consultation des réservations dans l'espace dédié

## 🎯 Fonctionnalités JavaScript

### Gestion de l'état
- Synchronisation temps réel avec le backend
- Mise à jour dynamique de l'interface
- Gestion des erreurs et feedback utilisateur

### API Calls
- Recherche de trajets
- Gestion du panier (ajout/suppression)
- Finalisation des réservations
- Consultation des réservations

### Validation
- Validation des dates (pas de dates passées)
- Vérification des champs obligatoires
- Gestion des cas d'erreur

## 🌐 Compatibilité navigateurs

- Chrome, Firefox, Safari, Edge (versions récentes)

## 🚀 Déploiement

Le frontend peut être déployé sur tout serveur web statique.
