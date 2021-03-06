# <%= module.name %> <%= module.version %>

<%= module.description %>

#### Stats

<%= stats.gzipSize %> | <%= stats.selectors.total %> | <%= stats.declarations.total %>
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev <%= module.name %>
```

#### With Git

```
git clone https://github.com/tachyons-css/<%= module.name %>
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "<%= module.name %>";
```

Then process the CSS using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons path/to/css-file.css > dist/t.css
```

#### Using the CSS

The built CSS is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/<%= module.name %>">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
<%= srcCss %>```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

<%= authors %>
## License

MIT
