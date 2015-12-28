# webfonts
une collection de webfonts libres, prêtes à l'emploi et optimisées pour le web :

- format `.woff2` prioritaire (alternatives en `.woff` et `.ttf` fournies)
- caractères latins, accents et devises uniquement (subsetting)
- hauteur de "x" adaptée pour fontes alternatives ajustées ("arial" pour fontes sans-serif et "georgia" pour fontes serif)
- fichier CSS `@font-face` fourni
- hack `?#iefix` pour éviter le chargement inutile de fichiers
- licences fournies

Exemple de `@font-face` fourni :

```css
/* Fonts */

@font-face {
    font-family: 'merriweather';
    src: url('merriweather-bold.woff2?#iefix') format('woff2'),
         url('merriweather-bold.woff') format('woff'),
         url('merriweather-bold.ttf') format('truetype');
    font-weight: bold;
    font-style: normal;
}
```

Usage :

```css
h1 {
  font-family: merriweather, georgia, serif;
}
```