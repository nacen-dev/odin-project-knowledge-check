# Webpack

## Knowledge Check

### How do you load CSS using webpack?

Using the style and css loader and placing this in the module object inside the rules array in the webpack.config.js file

```
module: {
  rules: [
    {
      test: /\.css$/i,
      use: ['style-loader', 'css-loader'],
    },
  ],
}
```

### How do you load images using webpack?

As of webpack 5 there is a built in asset modules that can be incorporated to load images, using this rule

```
{
  test: /\.(png|svg|jpg|jpeg|gif)$/i,
  type: 'asset/resource',
},
```

### How do you load fonts using webpack?

Similar to loading images it still uses the asset modules

{
test: /\.(woff|woff2|eot|ttf|otf)$/i,
type: 'asset/resource',
}

### How do you load data using webpack?

You will need a third party package to load the specific data for csv you can use the [csv-loader](https://github.com/theplatapi/csv-loader) and for xml you can use the [xml-loader](https://github.com/gisikw/xml-loader) then adding them as a rule

```
{
  test: /\.(csv|tsv)$/i,
  use: ['csv-loader'],
},
{
  test: /\.xml$/i,
  use: ['xml-loader'],
},
```

### How would you track errors in bundled source code?

Using the devtool property in webpack's config file and setting a sourcemap option, there are different [options](https://webpack.js.org/configuration/devtool/) to choose from.