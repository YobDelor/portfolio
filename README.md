# Portfolio — Yobouet Jean Luc Delor KASSIÉ

Refonte inspirée de **Escape Velocity** de HTML5 UP : composition éditoriale, bandeaux corail, en-tête bleu nuit, sections claires et navigation responsive.

## Lancer localement

Depuis ce dossier :

```bash
python -m http.server 8000
```

Puis ouvrir `http://localhost:8000`.

## Hébergement recommandé : Netlify

Ce portfolio est un site statique (HTML, CSS et JavaScript), sans commande de compilation. Netlify est recommandé ici parce qu'il héberge le site et prend aussi en charge le formulaire de contact.

### Option A — Déploiement connecté à GitHub (recommandé)

1. Décompresser l'archive et placer le contenu du dossier dans un dépôt GitHub.
2. Dans Netlify, choisir **Add new project** / **Import an existing project**, puis connecter GitHub et sélectionner le dépôt.
3. Comme le site n'utilise pas de framework ni d'étape de compilation, laisser la commande de build vide et définir le dossier publié sur la racine du dépôt (`.`).
4. Lancer le déploiement. Netlify fournira une URL publique en `netlify.app`.
5. Dans le tableau de bord du site, ouvrir **Forms** et activer **Form detection** si ce n'est pas déjà activé, puis redéployer le site.
6. Dans **Forms → Submission notifications**, ajouter une notification par e-mail et confirmer l'adresse destinataire si Netlify le demande.

Les prochains `git push` sur la branche de production déclencheront automatiquement un nouveau déploiement.

### Option B — Déploiement manuel

1. Décompresser l'archive.
2. Ouvrir la page de déploiement manuel Netlify : <https://app.netlify.com/drop>.
3. Glisser-déposer le dossier du site (celui qui contient directement `index.html`, `merci.html` et `assets/`).
4. Dans le tableau de bord du site, vérifier que **Forms → Form detection** est activé. Ajouter ensuite une notification e-mail dans **Forms → Submission notifications**.

Pour publier une mise à jour manuellement, glisser-déposer à nouveau le dossier mis à jour depuis la page **Deploys** du site.

## Formulaire de contact

Le formulaire est configuré avec **Netlify Forms** : il envoie les champs au service de formulaires de Netlify, sans ouvrir de logiciel de messagerie. La page `merci.html` s'affiche après une soumission réussie.

Le traitement du formulaire fonctionne sur un site déployé chez Netlify après activation de la détection des formulaires. En ouverture locale via `python -m http.server`, ou sur GitHub Pages / Cloudflare Pages sans service de formulaires supplémentaire, le formulaire ne pourra pas transmettre les messages.

Pour utiliser un autre hébergeur, remplacer Netlify Forms par un service compatible tel que Formspree, puis renseigner l'endpoint fourni par ce service.

## Contenu et personnalisation

- `index.html` : structure de la page, navigation, formulaire et sections.
- `merci.html` : page de confirmation après envoi du formulaire.
- `assets/css/style.css` : palette, mise en page, responsive, thème sombre et transitions.
- `assets/js/data.js` : compétences, projets et dépôts d'apprentissage.
- `assets/js/main.js` : rendu des cartes, filtres, recherche, thème et interactions visuelles.
- `assets/images/profile.jpg` : portrait.

Les projets dont le dépôt exact n'a pas pu être identifié sur les profils publics sont conservés, mais leur bouton GitHub indique « Dépôt à associer ». Remplacer ce champ par l'URL exacte lorsque le dépôt correspondant est public.

Les exercices et forks sont présentés séparément des projets originaux. Le dépôt KODJ est indiqué comme étant en développement, car son README GitHub le décrit encore comme un projet Flutter initial.

## Crédit du modèle

Design inspiré de [Escape Velocity](https://html5up.net/escape-velocity) par [HTML5 UP](https://html5up.net/), crédit conservé conformément à la licence [CC BY 3.0](https://html5up.net/license).
