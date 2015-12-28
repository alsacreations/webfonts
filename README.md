# webfonts collection

- parce que vous n'utilisez pas le CDN de Google Font ou Typekit (et que [vous avez probablement raison](http://www.alsacreations.com/article/lire/1695-partis-tiers-impacts-sur-la-vitesse-de-vos-sites.html)),
- parce que vous cherchez et installez vos fontes à la main,
- et qu'ensuite vous les adaptez et optimisez pour le web,
- systématiquement à chaque nouveau projet...

Alors il y a des chances que vous trouviez ici votre bonheur déjà prêt à l'emploi&nbsp;: une collection de fontes libres, prêtes à l'emploi et optimisées pour le web.

Les critères en considération pour figurer dans cette liste :
- être une fonte couramment employée sur le web, libre et gratuite
- proposer le format `.woff2` prioritairement (alternatives en `.woff` et `.ttf` fournies)
- se limiter aux caractères latins, accents et devises uniquement (subsetting)
- disposer d'hauteur de "x" adaptée pour fontes alternatives ajustées ("arial" pour fontes sans-serif et "georgia" pour fontes serif)
- proposer le fichier CSS `@font-face` fourni
- ajouter le hack `?#iefix` pour éviter le chargement inutile de fichiers sur les anciens IE
- ne pas tenir compte de IE8 et antérieur (pas de `.eot`, ils afficheront la fonte alternative)
- fournir les licences dans le dossier de fonte

*N'hésitez pas à proposer vos contributions de fontes, sous condition qu'elles respectent les critères ci-dessus.*

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