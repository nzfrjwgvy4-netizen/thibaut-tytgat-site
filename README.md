# Site — Thibaut Tytgat

Base statique pour un site vitrine de chef privé / chef à domicile.

## Lancer le site

Le site fonctionne sans build. Ouvre `index.html` directement ou utilise une extension VS Code comme Live Server.

Pour un serveur local avec Python :

```bash
python -m http.server 8000
```

Puis ouvre `http://localhost:8000`.

## Ajouter les photos

1. Place les photos dans `assets/images/`.
2. Ouvre `assets/js/config.js`.
3. Renseigne les chemins d’images, par exemple :

```js
images: {
  hero: "assets/images/hero.jpg",
  cuisine1: "assets/images/plat-01.jpg",
  cuisine2: "assets/images/plat-02.jpg",
  experience: "assets/images/service.jpg"
}
```

Aucune image externe ou générique n’est utilisée.

## Coordonnées

Dans `assets/js/config.js`, renseigne :

- `email`
- `whatsapp`
- `instagram`

Une fois l’email renseigné, le formulaire crée automatiquement un email prérempli via `mailto:`. Cela fonctionne sans backend. Pour une réception de formulaires plus professionnelle plus tard, un service gratuit de formulaires statiques peut être branché.

## Parcours / CV

Le contenu actuel est volontairement neutre. Il faut remplacer les blocs "À compléter" uniquement avec les informations du CV.

## Hébergement gratuit

Compatible notamment avec GitHub Pages, Cloudflare Pages ou Netlify, sans serveur applicatif.
