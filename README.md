# session-4
Styles et mise en forme

## Étapes

- [ ] Forker ce projet dans votre espace personnel sur Github
- [ ] Cloner le fork dans Github Desktop

Vous allez travailler sur le fichier styles.css, qui contiendra tous les styles du site internet composé de index.html, et des pages situées dans /pages. Le fichier styles.css contient déjà des styles pour gérer le positionnement des éléments.

- [ ] En utilisant au maximum la liste de propriétés CSS ci-dessous, et en utilisant les couleurs et les polices de votre choix, modifiez la feuille de styles générale du site.

Celui-ci doit s'approcher au maximum du rendu suivant : 

![]()

> Pensez à "aérer" votre code en sautant des lignes et en créant des indentations. Cela ne modifie pas le rendu et permet une meilleure lisibilité.

## Get started with CSS

Le CSS fait référence au HTML. Il désigne le contenu du site par le nom des balises HTML qui le structure.

Il peut s'écrire à plusieurs endroits : 

- Directement dans une balise HTML. Il est alors dit **Inline**. `<p style="font-size: 24px;">Ce paragraphe a une taille de caractères de 24 pixels</p>`
- Dans une page HTML, comme dans l'exemple ci-dessous. Il est alors dit **Interne**. 
```html
<html>
  <head>
    <style>
      p {
        font-size: 24px;
      }
    </style>
  </head>
  <body>
    <p>Tous les paragraphes ont une taille de caractères de 24 pixels</p>
  </body>
</html>
```
- Dans une feuille séparée, "appelée" de la manière suivante. Il est alors dit **Externe**.
```html
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="styles.css">
  </head>
  <body>
    <p>Tous les paragraphes ont une taille de caractères de 24 pixels</p>
  </body>
</html>
```
```css
p {
  font-size: 24px;
}
```

Le CSS (Cascading Style Sheets) est un **langage hiérarchique**, en cascade. 
- Les styles définis en derniers sont prioritaires sur ceux définis en amont.
  - Les styles définis de la manière la plus précise sont prioritaires sur ceux définis de manière générale.
   
Exemple : 

```css
p {
  color: red; /* Les paragraphes sont écrits en rouge */
}
article p {
  color: black; /* Les paragraphes dans les balises articles sont écrits en noir */
}
p {
  color: blue; /* Les autres paragraphes sont écrits en bleu */
}
```

D'une manière générale, on écrira les styles sur des feuilles **externes** et on s'arrangera pour écrire le moins de code possible. Les styles généraux de façon générale, et les choses les plus précises de manière précise.
