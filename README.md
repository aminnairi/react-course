# react-course

## Chapitre 1 : Hello, world!

Il est possible d'utiliser React sans aucun outils à l'aide de balises `script` et d'un lien vers la librairie.

### HTML

```bash
touch index.html
```

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Hello, world!">
    <meta name="theme-color" content="#FFFFFF">
    <title>Hello, world!</title>
  </head>
  <body>
    <div id="main"></div>
    <script src="https://unpkg.com/react@18/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js" crossorigin></script>
    <script src="./index.js"></script>
  </body>
</html>
```

### JavaScript

```bash
touch index.js
```

```javascript
const main = document.getElementById("main");
const root = ReactDOM.createRoot(main)
const element = React.createElement("h1", null, "Hello");

root.render(element);
```

### Navigateur

```bash
chromium index.html
```

## Exercice 1

Créer deux fichiers `index.html` et `index.js` et ajouter les lignes précédentes à ces fichiers. Testez votre code dans un navigateur pour et vérifier que vous ayez bien un titre qui apparaît à l'écran.
