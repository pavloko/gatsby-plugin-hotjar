# gatsby-plugin-hotjar

Easily add Hotjar Analytics to your Gatsby site.

## Install

`yarn add gatsby-plugin-hotjar`

## How to use

```javascript
// In your gatsby-config.js
plugins: [
  {
    resolve: `gatsby-plugin-hotjar`,
    options: {
      includeInDevelopment: false,
      id: YOUR_HOTJAR_ID,
      sv: YOUR_HOTJAR_SNIPPET_VERSION
    }
  }
];
```
