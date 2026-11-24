# My Invest. — SALTBURN CAPITAL

## Contenu
- `index.html` : application autonome
- `manifest.webmanifest` et `sw.js` : installation PWA et cache hors ligne
- `assets/` : icônes dérivées du visuel de coffre fourni

## Démarrage
Ouvrir `index.html` pour une utilisation locale. Pour l'installation PWA et le mode hors ligne, publier le dossier sur un hébergement HTTPS statique (par exemple GitHub Pages), puis ouvrir l'URL et utiliser le menu Installer / Ajouter à l'écran d'accueil.

## Données
Les données sont stockées dans `localStorage` du navigateur. Elles ne sont pas synchronisées entre appareils. Utiliser régulièrement l'export JSON pour sauvegarder et l'import JSON pour restaurer.

## Fonctionnement de l'historique
Chaque opération est conservée avec sa date. Les valorisations sont recalculées chronologiquement. Une opération de type « Définir la valorisation totale » fixe le montant de la catégorie à cette date. Le graphique global est reconstruit à partir de ces points.

## Limites de cette V1
- EUR uniquement.
- Valorisation manuelle : pas de connexion bancaire ou de cours de marché.
- Le patrimoine net correspond à la somme des huit catégories ; les dettes ne sont pas suivies séparément.
- Les données restent propres à un navigateur / appareil.
