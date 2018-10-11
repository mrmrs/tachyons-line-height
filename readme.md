# tachyons-line-height 3.0.7

Performance based css module.

### Stats

273 | 12 | 12
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev tachyons-line-height
```

Learn more about using css installed with npm:
* https://webpack.github.io/docs/stylesheets.html
* https://github.com/defunctzombie/npm-css

#### With Git

http:
```
git clone https://github.com/tachyons-css/tachyons-line-height
```

ssh:
```
git clone git@github.com:tachyons-css/tachyons-line-height.git
```

## Usage

#### Using with [Postcss](https://github.com/postcss/postcss)

Import the css module

```css
@import "tachyons-line-height";
```

Then process the css using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons path/to/css-file.css > dist/t.css
```

#### Using the css

##### CDN
The easiest and most simple way to use the css is to use the cdn hosted version. Include it in the head of your html with:

```
<link rel="stylesheet" href="http://unpkg.com/tachyons-line-height@3.0.7/css/tachyons-line-height.min.css" />
```

##### Locally
The built css is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/tachyons-line-height">
```

#### Development

The source css files can be found in the `src` directory.
Running `$ npm start` will process the source css and place the built css in the `css` directory.

## The css

```css
/*

   LINE HEIGHT / LEADING
   Docs: http://tachyons.io/docs/typography/line-height

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/
.lh-solid { line-height: 1; }
.lh-title { line-height: 1.25; }
.lh-copy { line-height: 1.5; }
@media screen and (min-width: 30em) {
 .lh-solid-ns { line-height: 1; }
 .lh-title-ns { line-height: 1.25; }
 .lh-copy-ns { line-height: 1.5; }
}
@media screen and (min-width: 30em) and (max-width: 60em) {
 .lh-solid-m { line-height: 1; }
 .lh-title-m { line-height: 1.25; }
 .lh-copy-m { line-height: 1.5; }
}
@media screen and (min-width: 60em) {
 .lh-solid-l { line-height: 1; }
 .lh-title-l { line-height: 1.25; }
 .lh-copy-l { line-height: 1.5; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

ISC

