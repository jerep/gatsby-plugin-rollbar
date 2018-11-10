# gatsby-plugin-rollbar

Gatsby plugin to add Rollbar error tracking to your site.

Learn more about Rollbar [here](https://rollbar.com).

## Install

`npm install --save gatsby-plugin-rollbar`

## How to use

```javascript
// In your gatsby-config.js
plugins: [
  {
    resolve: "gatsby-plugin-rollbar",
    options: {
      accessToken: "YOUR_ROLLBAR_ACCESS_TOKEN",
      // For all configuration options, see https://docs.rollbar.com/v1.0.0/docs/rollbarjs-configuration-reference
      captureUncaught: true,
      captureUnhandledRejections: true,
      payload: {
        environment: "production"
      }
    }
  }
];
```
