# Bristol Marine — site mis à jour

Refonte partielle : ajout de la section **Location** (Sans permis / Avec permis / Avec skipper),
d'un sélecteur de langue **FR / EN / IT**, et d'une **barre mobile** Appeler · WhatsApp · Réserver.
Tout le reste du site (Maison, Métiers, Charter yachts, Vente, Contact) est conservé.

## Fichiers à mettre en ligne

| Élément | Rôle |
|---|---|
| `index.html` | La page complète. |
| `logo.png` | Logo Bristol Marine Green détouré (fond transparent). |
| `f/` | Les 34 photos de la flotte (une par vue, rangées par bateau). |

Déposer **index.html**, **logo.png** et le dossier **f/** à la racine du dépôt GitHub,
en écrasant l'ancien `index.html`. Vercel redéploie automatiquement.

## La section Location

- Trois onglets : Sans permis · Avec permis · Avec skipper.
- Chaque bateau a sa galerie photo (flèches + points), sa description (bouton « Voir le détail »),
  ses équipements, ses tarifs et ses informations.
- Tarifs : grille pour le FUN YAK, le Quicksilver, les deux Bénéteau permis et le Cap Camarat ;
  grille journée/demi-journée/sunset pour le Flyer 750 SD ; « Tarif sur demande » pour les cinq autres skippers.
- Boutons **Réserver** (ouvre un courriel prérempli vers contact@bristolmarine.fr) et **WhatsApp**.

## Le FUN YAK

Ses photos ne sont pas encore fournies : la fiche affiche « Photos à venir ».
Dès que les clichés sont prêts, les déposer dans `f/` sous les noms `funyak-1.jpg`, `funyak-2.jpg`…
puis ajouter ces noms dans le tableau `photos: []` du FUN YAK, à l'intérieur de `index.html`
(chercher `id: "funyak"`).

## Les langues

Le sélecteur FR/EN/IT en haut à droite traduit la section Location et les éléments de réservation.
Les sections patrimoniales (histoire, vente de yachts) restent en français pour l'instant ;
elles pourront être traduites dans un second temps.

## Modifier un texte ou un tarif

Tout est dans `index.html`, dans le bloc `const LOCATION = { … }`.
Chaque texte existe en trois langues (`fr`, `en`, `it`) : modifier les trois.

## Coordonnées

Téléphone / WhatsApp : 06 12 79 72 47 · E-mail : contact@bristolmarine.fr · Port des Fourmis, Beaulieu-sur-Mer.
