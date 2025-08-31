# Z‑Event 2025 – Multi‑flux

## Présentation
Cette page HTML permet de suivre **plusieurs streamers Twitch du Z‑Event** en simultané sur une seule interface. Elle a été conçue pour simplifier le suivi de l’événement : ajouter/supprimer des chaînes, mettre un flux en **focus** avec son **chat**, et mémoriser vos choix d’une session à l’autre.

## Fonctionnalités
- **Grille de flux vidéo** responsive (colonnes auto, 2, 3 ou 4).
- **Liste des participants 2025** pré‑enregistrée (plateau Montpellier).
- Ajout possible de **n’importe quelle chaîne Twitch** manuellement.
- **Focus** : un clic sur « Focus » affiche la vidéo + le chat en haut (2/3 + 1/3), tout en conservant la vignette.
- **Enlever le focus** via un bouton ou la touche *Échap*.
- **Persistance** automatique : les chaînes sélectionnées et le nombre de colonnes sont sauvegardés dans le navigateur.
- **Première ouverture** : la chaîne **ZeratoR** est affichée par défaut.
- **Lien direct** vers la [page officielle du Z‑Event](https://www.zevent.fr).
- **Option cagnotte** (désactivée par défaut) : possibilité d’afficher un compteur si une **URL JSON publique** est fournie (rafraîchissement toutes les 15 s).

## Installation et utilisation
1. Téléchargez le fichier `index.html` (contenu fourni dans ce dépôt).
2. Hébergez‑le :
   - En local :
     ```bash
     npx serve
     # ou
     python -m http.server 8080
     ```
     Puis ouvrez [http://localhost:8080](http://localhost:8080).
   - Ou bien via **GitHub Pages** ou tout autre hébergement statique.
3. La première fois, seul **ZeratoR** s’affiche.
4. Ajoutez/supprimez des flux depuis la barre d’outils.
5. Cliquez sur **Focus** pour mettre un streamer en avant avec son chat.
6. Fermez le focus avec le bouton « Enlever le focus » ou *Échap*.

⚠️ **Important** : l’intégration Twitch impose que le champ `parent` corresponde au domaine utilisé. Cela signifie qu’il faut impérativement ouvrir la page via un domaine valide (pas `file://`).

## Option « Cagnotte »
- Si une **source JSON publique** est disponible (par exemple un endpoint fourni par l’organisation), collez son URL dans le champ prévu, puis cliquez sur **Activer**.
- Le compteur apparaîtra en haut de la page.
- Cliquez sur **Désactiver** pour le masquer.

## Licence
Projet à usage personnel/communautaire pendant le **Z‑Event 2025**. Aucune garantie sur la disponibilité des flux ou des API externes.

