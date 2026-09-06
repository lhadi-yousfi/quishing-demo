# 🎯 Guide d'animation – semaine de sensibilisation cybersécurité

## Ce que vit un collègue qui scanne (environ 5 minutes)

1. Son téléphone ouvre une page noire façon « terminal de hacker » : connexion à l'appareil,
   extraction des contacts, copie des photos, récupération des mots de passe… (8 secondes).
2. Flash, vibration, écran rouge : **« Votre téléphone a été piraté »**, avec son type de
   téléphone et l'heure affichés. Un bouton « Que faire maintenant ? » apparaît (et l'écran
   suivant arrive tout seul après quelques secondes, au cas où).
3. **« Respirez, rien de tout ça n'est vrai »** : c'est la campagne de sensibilisation de
   l'entreprise. Rien n'a été lu ni transmis. Explication de ce qu'un vrai QR piégé aurait pu faire.
4. **Quiz de 10 questions**, une à la fois, avec explication immédiate à chaque réponse.
5. **Résultat** : score, niveau (Cyber-apprenti → Cyber-expert), les 6 règles d'or, et un bouton
   pour partager la démo à un collègue.

## Avant la semaine (J-7 à J-1)

1. **Mettre la page en ligne** (voir `README.md`) et la tester sur 2 téléphones (iPhone + Android).
2. **Personnaliser** le nom de l'entreprise et le contact informatique dans `index.html` (bloc `CONFIG`).
3. **Informer** la direction, le service informatique / RSSI et, si besoin, les représentants du
   personnel : c'est un exercice pédagogique, sans collecte de données, sans piège individuel.
4. **Imprimer** :
   - 3 à 5 affiches A4 (`affiche.html`) : cafétéria, hall, machine à café, ascenseur, parking.
   - 1 planche d'autocollants (`affiche.html` → *Planche d'autocollants*) : tables, tableau
     d'affichage, WC, porte-manteaux.
   - Les fiches mémo (`fiche-memo.html`), 1 par collaborateur.
5. **Tester chaque impression** avec votre téléphone.
6. Préparer la phrase de débriefing : *« Ce n'était pas une vraie attaque, personne n'est pointé
   du doigt, voici ce qu'on retient. »*

## Pendant la semaine

- **Lundi** : poser les affiches sans annonce. La surprise fait partie de l'apprentissage.
- **Chaque jour** : vérifier discrètement que les affiches sont en place.
- **Mercredi** : message à toute l'équipe :
  > « Vous avez peut-être scanné un QR code cette semaine (café offert, Wi-Fi…) et vu un écran
  > inquiétant. C'était une démonstration organisée en interne pour la semaine cybersécurité.
  > Aucune donnée n'a été collectée. Si vous ne l'avez pas encore fait, tentez le quiz ! »
- **Vendredi** : débriefing de 15 minutes et distribution des fiches mémo.

## Débriefing (15 minutes)

1. **Scanner l'affiche en direct** (2 min), téléphone projeté si possible. Laisser la séquence
   de piratage se dérouler : les réactions dans la salle font le travail.
2. **Question ouverte** : *« Qu'est-ce qui aurait pu vous mettre la puce à l'oreille avant de
   scanner ? »* (3 min). Laisser parler, sans juger.
3. **Faire le quiz collectivement** à l'écran, en votant à main levée sur 3 ou 4 questions (6 min).
   Les questions « e-mail piégé » et « code SMS reçu sans rien demander » font toujours débat.
4. **Montrer l'aperçu d'URL** de l'appareil photo : scanner, s'arrêter sur la bulle qui affiche
   le lien, la lire à voix haute (2 min).
5. **Message clé** (1 min) : *un QR code n'est qu'un lien déguisé. Et si on s'est fait avoir, on
   change son mot de passe tout de suite et on prévient l'informatique. Personne ne vous en voudra.*
6. **Distribuer la fiche mémo** (1 min).

## Ton à adopter

- Bienveillant, jamais culpabilisant : « ça marche sur tout le monde », « l'important c'est le réflexe ».
- Pas de statistiques individuelles, pas de « qui a scanné ». La page ne le sait pas, et c'est voulu.
- Valoriser ceux qui ont signalé un QR suspect : c'est exactement le comportement recherché.

## Variantes possibles

- **Escalade** : changer l'affiche en milieu de semaine (café → jeu-concours) pour montrer que
  l'accroche varie mais que le mécanisme est le même.
- **Le faux par-dessus le vrai** : coller l'autocollant de démo *par-dessus* un vrai QR (menu de
  la cantine, par exemple) pour illustrer le signal d'alerte n°1. Retirez-le en fin de semaine.
- **Atelier en salle** : ouvrir `index.html#quiz` sur le vidéoprojecteur et faire le quiz en équipe.
- **Défi** : « Qui obtient 10/10 ? » Le résultat s'affiche à l'écran, chacun peut le montrer.

## Après la semaine

- Retirer toutes les affiches et autocollants.
- Envoyer un dernier message avec le lien de la démo pour que chacun la montre à ses proches.
- Optionnel : dépublier le site (*Settings → Pages → Unpublish site*) ou le garder pour les
  nouveaux arrivants.
