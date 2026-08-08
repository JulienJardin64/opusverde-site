# Site vitrine Opus Verde

Site statique de présentation (4 pages) pour `opusverde.fr`.

## Contenu

- `index.html` — Accueil / présentation
- `fonctionnalites.html` — Fonctionnalités
- `tarifs.html` — Tarifs
- `styles.css` — feuille de style commune
- `main.js` — menu mobile + animations au scroll
- `logo-opusverde.png` — logo (version foncée, pour l'en-tête / fonds clairs)
- `logo-opusverde-clair.png` — logo (version claire, pour le pied de page / fonds foncés)
- `logo-mark.png` — la marque seule (papillon sans texte), utile pour un favicon

Aucune dépendance, aucun build : ce sont des fichiers HTML/CSS/JS purs.
Les seules ressources externes sont les polices Google (Space Grotesk + Inter),
chargées automatiquement.

## Les boutons "Ouvrir l'application"

Ils pointent tous vers `https://appli.opusverde.fr` (ta version validée).

## Déployer sur Vercel (nouveau projet séparé)

1. Crée un nouveau dépôt GitHub (ex. `opusverde-site`) et pousse-y ces fichiers,
   OU place-les dans un sous-dossier `/site` de ton dépôt existant.
2. Sur Vercel → **Add New… → Project** → importe ce dépôt.
3. Framework Preset : **Other** (site statique, pas de build).
   - Build Command : laisser vide
   - Output Directory : laisser vide (racine)
4. Déploie. Vercel te donne une URL temporaire `xxx.vercel.app` pour vérifier.
5. Quand tout est bon → Settings → Domains → ajoute `opusverde.fr`
   (et retire-le de l'ancien projet applicatif au préalable).

## Personnalisation rapide

- **Logo** : ton logo officiel est intégré (fond détouré/transparent).
  Deux versions sont utilisées automatiquement : `logo-opusverde.png` (foncée)
  dans l'en-tête, `logo-opusverde-clair.png` (claire) dans le pied de page.
  Pour ajuster leur taille, voir `.brand__logo` dans `styles.css`.
- **Email de contact** : recherche `contact@opusverde.fr` dans les fichiers et
  remplace si tu utilises une autre adresse.
- **Téléphone** : `06 46 41 78 04` dans `contact.html` (et le lien `tel:`).
- **Couleurs / typo** : tout est centralisé en haut de `styles.css`
  (variables `--brand-500`, `--forest-900`, etc.).
