# 🛡️ Campagne de sensibilisation au quishing (QR code piégé) + quiz cybersécurité

Page web autonome (un seul fichier HTML, sans backend) à héberger sur GitHub Pages.
Un collègue scanne le QR code imprimé et vit ce déroulé sur son téléphone :

1. **☠️ « Votre téléphone a été piraté »** : une fausse séquence de piratage (terminal, barres de
   progression, alarme rouge, type d'appareil affiché). Ça fait peur… pendant quelques secondes.
2. **😮‍💨 « Respirez, rien de tout ça n'est vrai »** : c'est une campagne de sensibilisation.
   Explication de ce qu'un vrai attaquant aurait pu faire (quishing).
3. **🎯 Quiz interactif de 10 questions** (QR codes, phishing, mots de passe, double
   authentification, clé USB, appel frauduleux, verrouillage, signalement), avec explication
   à chaque réponse, score, niveau, confettis et les 6 règles d'or à retenir.

**Aucune donnée n'est lue, stockée ni transmise.** Les seules informations affichées (type
d'appareil, navigateur, heure) sont lues localement par le navigateur et ne quittent pas le
téléphone. Les nombres de contacts / photos « copiés » sont tirés au hasard. Aucune marque
réelle n'est imitée.

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `index.html` | **La démo** : piratage simulé → soulagement → quiz → résultat. C'est vers ce fichier que pointe le QR imprimé. |
| `affiche.html` | Affiches A4 prêtes à imprimer (café offert, Wi-Fi invité, jeu-concours, planche de 6 autocollants). Le QR est généré automatiquement. |
| `fiche-memo.html` | Fiche mémo A5 (2 par page A4) à distribuer aux collègues après la campagne. |
| `GUIDE-DEMO.md` | Déroulé conseillé de la semaine et du débriefing. |
| `.nojekyll` | Indique à GitHub Pages de publier les fichiers tels quels. |

## Personnaliser en 30 secondes

Ouvrez `index.html` et modifiez les deux lignes du bloc `CONFIG` (vers la ligne 250) :

```js
var CONFIG = {
  entreprise: 'votre entreprise',          // ex. 'Dupont Industries'
  contactIT:  'le service informatique'    // ex. 'le support IT (poste 4242)'
};
```

Les questions du quiz sont dans le tableau `QUIZ` juste en dessous : texte, options, index
de la ou des bonnes réponses (`a`), explication (`why`). Ajoutez, retirez ou modifiez librement.

## Mise en ligne sur GitHub Pages (5 minutes)

1. Sur https://github.com, bouton **« + »** en haut à droite → **New repository**.
2. Nom : `quishing-demo`. Visibilité : **Public**. **Create repository**.
3. Cliquez **uploading an existing file**, glissez-déposez **les 6 fichiers** de ce dossier
   (les fichiers, pas le dossier), puis **Commit changes**.
4. **Settings → Pages** (menu de gauche).
5. *Build and deployment* : Source = **Deploy from a branch**, Branch = **main**, dossier **/ (root)**, **Save**.
6. Attendez 1 à 2 minutes, rechargez : l'adresse s'affiche, de la forme
   `https://VOTRE-COMPTE.github.io/quishing-demo/`
7. Ouvrez-la sur votre téléphone : la séquence de piratage doit démarrer toute seule.

> Pour modifier plus tard : ouvrez le fichier sur GitHub, crayon ✏️, collez le nouveau contenu,
> **Commit**. En ligne au bout d'une minute.

## Imprimer les QR codes et les affiches

Une fois le site en ligne, **depuis un ordinateur** :

- **Affiches** : `https://VOTRE-COMPTE.github.io/quishing-demo/affiche.html`.
  L'adresse de la démo est pré-remplie et le QR déjà généré. Choisissez le modèle, **Imprimer**
  (ou « Enregistrer au format PDF » dans la boîte d'impression).
- **Fiches mémo** : `.../fiche-memo.html`, **Imprimer**, découper le long des pointillés.
- **QR seul (PNG)** : `.../index.html#generateur`, bouton **Télécharger en PNG**.

Conseils : QR de 5 cm minimum, marge blanche, papier mat. Testez chaque impression avec
votre téléphone avant de l'afficher.

## Accès directs pour l'organisateur

| Adresse | Ouvre |
|---|---|
| `.../index.html` | La démo complète (ce que voient les collègues) |
| `.../index.html#quiz` | Directement le quiz (pour un atelier en salle) |
| `.../index.html#generateur` | Le générateur de QR |

## Confidentialité

- Aucun formulaire, aucun envoi réseau, aucun cookie, aucun stockage.
- Seule ressource externe : la librairie `qrcode-generator` chargée depuis cdnjs, utilisée
  uniquement par le générateur et les affiches. La démo et le quiz fonctionnent sans elle.
- Prévenez la direction et l'équipe informatique avant la campagne.
- Après la campagne, retirez les affiches et, si vous le souhaitez, dépubliez le site
  (*Settings → Pages → Unpublish site*).
