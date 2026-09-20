# Radar Stages Tech

Tableau de bord de veille des offres de stage / alternance (Account Management, SDR, BDR, Account Executive) chez ~100 entreprises tech ciblées — France & Europe (+ Hong Kong, Singapour, États-Unis pour les Summer Internships).

## Contenu
- `index.html` — la page du tableau de bord (HTML/CSS/JS autonome : tiers S/A/B/Bonus/FR, filtres par rôle et par tier, badges Stage/Alternance, statut de dernière vérification).

## Important : d'où viennent les données
Les offres ne sont **pas** dans ce dépôt. La page lit sa base de données via la capacité `db` des Artifacts Claude (`claude.use("db")`), alimentée à chaque passage par la tâche planifiée de veille.
Hébergée ailleurs (ex. GitHub Pages), la page s'ouvre mais affiche uniquement les **lignes d'exemple** — pas de données réelles. Ce dépôt sert de sauvegarde / versionnage du code.

## Version live
Le tableau de bord fonctionnel est publié comme Artifact Claude (privé, lié à ton compte).
