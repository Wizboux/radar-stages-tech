# Radar Stages Tech

Tableau de bord de veille des offres de stage / alternance (Account Management, SDR, BDR, Account Executive) chez ~100 entreprises tech ciblées — France & Europe (+ Hong Kong, Singapour, États-Unis pour les Summer Internships).

## Contenu
- `index.html` — la page du tableau de bord (HTML/CSS/JS autonome : tiers S/A/B/Bonus/FR, filtres par rôle et par tier, badges Stage/Alternance).
- `data.json` — instantané des offres vérifiées (`generatedAt`, `status`, `listings`). La page le lit quand elle est ouverte hors de Claude.

## Voir la page
Il faut la servir en HTTP (un simple double-clic sur `index.html` ne peut pas charger `data.json`) :
- **GitHub Pages** : Settings → Pages → Deploy from a branch → `main` / root. Sur un compte gratuit, le dépôt doit être public.
- **En local** : `python3 -m http.server` dans le dossier, puis http://localhost:8000

## D'où viennent les données
La source de vérité est la base de l'Artifact Claude, alimentée par la tâche planifiée de veille. `data.json` en est une copie : elle n'est à jour qu'au moment où on la régénère et qu'on la pousse. La date de l'instantané est affichée en haut de la page.
