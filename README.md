This is a [webpack](http://webpack.js.org/) plugin powered by [HTML Webpack Plugin](https://github.com/jantimon/html-webpack-plugin), and add just one boolean param to the options.

**webpack.config.js**
```js
const HtmlWebpackPlugin = require('html-webpack-plugin')

module.exports = {
  plugins: [
    new HtmlWebpackPlugin({
      vue: true
    })
  ]
}
```

This will generate a file `dist/index.html` containing the following

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Webpack App</title>
  </head>
  <body>
    <div id="app"></div>
    <script src="index_bundle.js"></script>
  </body>
</html>
```
This param add entry point for Vue.js app.
