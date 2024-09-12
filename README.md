# gatsby-plugin-hotjar

Easily add Hotjar Analytics to your Gatsby site.

## Install

`yarn add gatsby-plugin-hotjar`

or

`npm i gatsby-plugin-hotjar --save`

## How to use

```javascript
// In your gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: "gatsby-plugin-hotjar",
      options: {
        includeInDevelopment: true, // optional parameter to include script in development
        addToHead: false, // optional parameter to append script to the head instead of the body
        id: YOUR_HOTJAR_ID,
        sv: YOUR_HOTJAR_SNIPPET_VERSION,
      },
    },
  ],
};
```

To find your Hotjar ID, click the **Tracking code** button for your site. The Hotjar Snippet Version is in the tracking code, look for a line like:

```javascript
h._hjSettings={hjid:[hotjar id],hjsv:6};
```

The version is the value of `hjsv`.
