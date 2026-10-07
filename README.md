# 🌦️ Appli météo — JavaScript & API OpenWeather

> Petite application qui affiche la météo d'une ville en interrogeant l'**API OpenWeather** avec `fetch` et `async/await`.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

---

## 📖 À propos

Exercice réalisé pendant ma formation de **Développeuse Web et Web Mobile (DWWM)** pour apprendre à consommer une API REST depuis le navigateur.
Le projet contient deux pages :

| Page | Ce qu'elle affiche | Point d'accès de l'API |
|---|---|---|
| `meteo-actuelle.html` | Température, humidité, vent, nuages, description et icône du moment | `/data/2.5/weather` |
| `index.html` | Tableau des prévisions sur 5 jours, par tranche de 3 heures | `/data/2.5/forecast` |

## 🧠 Ce que j'ai travaillé

- Appels HTTP avec **`fetch`** et **`async` / `await`**
- Gestion des erreurs avec `try` / `catch` et vérification de `response.ok`
- Lecture d'une réponse **JSON** et parcours d'un tableau avec `forEach`
- Conversion des dates Unix en dates lisibles (`new Date(dt * 1000).toLocaleString("fr")`)
- Mise à jour dynamique du **DOM** (génération des lignes du tableau)
- Événements clavier et clic (`keypress`, `click`)
- Tableau mis en forme avec **Bootstrap**

## 🚀 Lancer le projet

1. Créez un compte gratuit sur [openweathermap.org](https://openweathermap.org/api) et récupérez une clé API.
2. Clonez le dépôt :
   ```bash
   git clone https://github.com/aurored2-star/meteo-api.git
   cd meteo-api
   ```
3. Copiez `config.example.js` en `config.js` et collez-y votre clé :
   ```js
   const API_KEY = "votre_cle_ici";
   ```
4. Ouvrez `index.html` dans votre navigateur (ou avec **Live Server** dans VS Code), tapez une ville et appuyez sur **Entrée**.

> 🔐 `config.js` est listé dans `.gitignore` : la clé API reste sur votre machine et n'est jamais publiée sur GitHub.

## 🔧 Pistes d'amélioration

- [ ] Regrouper les deux pages en une seule interface (météo actuelle + prévisions)
- [ ] Afficher un message à l'utilisateur quand la ville n'existe pas
- [ ] Ajouter un bouton « Rechercher » à côté du champ de saisie
- [ ] Géolocaliser l'utilisateur pour afficher sa météo automatiquement

## 👩‍💻 Autrice

**Aurore Dufour**, développeuse web & mobile en formation
[GitHub](https://github.com/aurored2-star)
