Integrating Nord’s themes into your project is straightforward. To get started, add one of the following link tags to the  `<head>`  of your application:

  
Theme: Dark default

```html
<!-- Dark default theme --><link rel="stylesheet" href="https://nordcdn.net/ds/themes/7.0.3/nord-dark.css" integrity="sha384-NapCEph0LBSHkah3OjDmMM+r1L57btHpjsuxi1CM7Cxn9da8H8lHYXwgD8KvtlE5" crossorigin="anonymous" />
```

Copy to clipboard

When using Nord’s themes, it’s required to include our CSS Framework  _before_  the theme link tag to get access to properties such as margin, padding, font sizes, and similar which are not bundled into each theme:

```html
<link rel="stylesheet" href="https://nordcdn.net/ds/css/2.4.1/nord.min.css" integrity="sha384-7yCjjICdCmNLaOvslgtJXsmXDQehOXxb8YW+FQni9dmtkaOspP9zIDmijNI38BAq" crossorigin="anonymous" />
```


Please note that the  **Light Default Theme**  is bundled into our  [CSS framework](https://nordhealth.design/css/), meaning there is no need to add this theme if you already have the CSS Framework installed and it’s the only theme you wish to use.

----------

## Installation

While usage through Nord CDN is the fastest way to get started, we also support installing any of the themes locally using npm. Before you move further with this approach, please make sure you have  [Node.js](https://nodejs.org/en/)  installed on your machine. You can install the latest version through their website.

If you’re planning on using Nord Themes in a project that doesn’t yet use  [npm](https://www.npmjs.com/), you’ll first need to create a  [package.json](https://docs.npmjs.com/files/package.json)  file. To do this, run  `npm init`  and follow the steps provided. Once finished, you can continue the Nord Themes installation by following the instructions below.

### Install using npm

Run in your project or website root directory (where package.json lives):

```shell
npm install @nordhealth/themes @nordhealth/css --save
```


### Importing a theme locally

Once you’ve installed our npm packages, you can then import any of Nord’s themes into your project as CSS, SCSS, Sass or Less:

  

Theme: Dark default

```scss
/* Import default dark theme */@import "~@nordhealth/css/lib/nord.min.css";@import "~@nordhealth/themes/lib/nord-dark.css";
```


If you’re not using  [Webpack](https://webpack.github.io/)  or a similar tool for your build process, you may have to provide the full paths to Node Modules:

```scss
@import "/node_modules/@nordhealth/css/lib/nord.min.css";@import "/node_modules/@nordhealth/themes/lib/nord-dark.css";
```

----------

## Available themes

Below you can find a list of available themes and paths to them inside our Node.js package:

-   **Light default:**  `@nordhealth/themes/lib/nord.css`
-   **Light high contrast:**  `@nordhealth/themes/lib/nord-high-contrast.css`
-   **Dark default:**  `@nordhealth/themes/lib/nord-dark.css`
-   **Dark high contrast:**  `@nordhealth/themes/lib/nord-dark-high-contrast.css`

### Themes on Nord CDN

```html
<!-- Light default theme --><link rel="stylesheet" href="https://nordcdn.net/ds/themes/7.0.3/nord.css" integrity="sha384-SXaLtUT8XJ2GLBBLxVdURI2G6uY/lshRBSAINRGNFUmnj0wUcJmKv6Br/U2BJqTb" crossorigin="anonymous" /><!-- Light high contrast theme --><link rel="stylesheet" href="https://nordcdn.net/ds/themes/7.0.3/nord-high-contrast.css" integrity="sha384-eu7xhLEB/h23VTImjvtkKlj6QZxpEjBXm+mcMoy2+xofDDAM9H5xxEvdgA1AxomP" crossorigin="anonymous" /><!-- Dark default theme --><link rel="stylesheet" href="https://nordcdn.net/ds/themes/7.0.3/nord-dark.css" integrity="sha384-NapCEph0LBSHkah3OjDmMM+r1L57btHpjsuxi1CM7Cxn9da8H8lHYXwgD8KvtlE5" crossorigin="anonymous" /><!-- Dark high contrast theme --><link rel="stylesheet" href="https://nordcdn.net/ds/themes/7.0.3/nord-dark-high-c
```


> Written in [Markdown](https://code.visualstudio.com/docs/languages/markdown) by codemikko is using [vsCode](https://code.visualstudio.com)
