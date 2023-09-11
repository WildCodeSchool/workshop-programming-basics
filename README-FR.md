# Calculatrice simple

[⬅ English version](./)

Nous allons explorer les principes fondamentaux de JavaScript en construisant une calculatrice. Vous allez donc apprendre à manipuler des variables, des opérateurs, des conditions...

## Mise en place de l'atelier

Pré-requis : [JS Basics 01](https://odyssey.wildcodeschool.com/quests/1262), [JS Basics 02](https://odyssey.wildcodeschool.com/quests/1267)
{: .alert-info}

Important : les premières étapes sont à faire avec votre terminal !
{: .alert-warning}

Créez un nouveau dossier `simple-calculator` et créez un fichier `index.html` vide à l’intérieur.

Ouvrez `index.html` avec VSCode et ajoutez la structure HTML5.

Dans la balise `<body>` ajoutez une balise `<script>` avec le code suivant :

```js
console.log("Hello wilders!");
```

Ouvrez le fichier `index.html` dans un navigateur, et afficher la console (F12), que voyez-vous ? Si vous voyez votre message ci-dessus, cela signifie que tout fonctionne bien !

Pour être sûr, expliquez ce que vous avez fait à vos collègues.

### Ce que vous obtenez

Voilà la structure HTML5 de base ainsi que l’ajout de la balise `<script>` avec le code `console.log("Hello les wilders!");` :

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Simple calculator</title>
  </head>
  <body>
    <script>
      console.log("Hello wilders!");
    </script>
  </body>
</html>
```

Dans l'inspecteur :

!["Hello les wilders!" dans l'inspecteur](./images/helloWilders.png)

## Les premières instructions

Pré-requis : [JS Basics 03](https://odyssey.wildcodeschool.com/quests/1268), [JS Basics 04](https://odyssey.wildcodeschool.com/quests/1269)
{: .alert-info}

La première étape de la création de notre calculatrice consiste à **instancier** des variables.

Créez 3 variables :

- `firstValue` : par défaut, le nombre `1` sera affecté.
- `operator` : nous allons utiliser le symbole `"+"`.
- `secondValue` : nous allons affecter le nombre `2`.

Maintenant, vous allez faire autant de `console.log` que vous avez de variable. Que voyez-vous ?

Et si on demande l’avis de l’utilisateur ? Nous allons utiliser la fonction `prompt` (voir [la documentation](https://developer.mozilla.org/en-US/docs/Web/API/Window/prompt)) et assigner des valeurs choisies par l'utilisateur à nos variables. (Attention, pas `operator`, juste les valeurs)

Qu’affichent les `console.log` ?

### On comprend la console

Ajoutez un `console.log` de `firstValue + secondValue` : qu’affiche t-il ? Pourquoi ? Que devons-nous faire ? Conseil : regardez [cette documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt).

Et maintenant, qu’affiche le `console.log` ? Pourquoi ?

Pour être sûr, expliquez ce que vous avez fait à vos collègues.

## On agit sur l'opérateur

Pré-requis : [JS Basics 05](https://odyssey.wildcodeschool.com/quests/1270)
{: .alert-info}

Un peu de ménage : supprimez tous les `console.log`.

Vous allez ajouter une condition sur la variable de l’opérateur :

- Si elle contient la valeur `"+"` alors, nous allons _additionner_ les deux valeurs, stocker le résultat dans une variable `result`, à afficher dans un `console.log`.
- Sinon, dans tous les autres cas, nous allons _soustraire_ les deux valeurs, stocker le résultat dans une variable `result`, à afficher dans un `console.log`.

Expliquez ce que vous avez fait à vos collègues.

## Dernières instructions

Pré-requis : [JS Basics 05](https://odyssey.wildcodeschool.com/quests/1270)
{: .alert-info}

Vous avez presque fini, maintenant que vous avez fait une première condition, ajoutez les conditions pour _tous les opérateurs_ :

- Modifier votre code et ajoutez des conditions pour les opérateurs `"-"`, `"*"` et `"/"` : pensez à la construction `else if`.
- Dans chaque cas, affichez le résultat de l’opération mathématique correspondante avec un `console.log`.
- Ajoutez un cas par défaut avec un `else` final qui affiche `"Opérateur non valide"`.

☆ Pré-requis : [JS Basics 06](https://odyssey.wildcodeschool.com/quests/1278)
{: .alert-info}

**☆ Bonus :** Déplacez tout le code dans une fonction pour le rendre réutilisable.

# Le juste prix

Pour les personnes très motivées 🤘
{: .alert-warning}

## Vous aimez jouer ?

Alors c’est le moment de créer un petit jeu !

Mêmes étapes que pour la partie [“Mise en place de l'atelier”](#mise-en-place-de-latelier), vous n’avez qu’à changer le nom du dossier.

- Demandez le nom du joueur ou de la joueuse.
- Stockez un nombre aléatoire entre 1 et 100 (le prix à trouver).

cadeau : `const rightPrice = Math.ceil(Math.random() * 100);`
{: .alert-info}

- Demander un nombre au joueur ou à la joueuse (entre 1 et 100).
- Si le nombre est supérieur au juste prix, affichez `"C’est moins"`.
- Si le nombre est inférieur au juste prix, affichez `"C’est plus"`.
- Si le nombre est égal au juste prix, affichez `"Bravo <nom> tu as gagné !"` avec `<nom>` qui est remplacé par le nom "prompté" au début du jeu.

Le jeu s’arrête lorsque c’est gagné.
