# CSS loader

> A couple of simple examples of loaders using only one `div` and *CSS*.

![loader-g](https://cloud.githubusercontent.com/assets/1345662/19414412/5e472d6c-9322-11e6-9407-5e3662072aee.gif)

[Try it online! :metal:](http://www.raphaelfabeni.com.br/css-loader/)

## Why

Usually it's common to show a loader to the users when they must wait something in a web application (an _ajax_ request or a form submit, etc). _Gif_image loaders was great but using CSS we can avoid the image request, also it's easier for customise and maintain and it's more cool.

## Install

```bash
npm install pure-css-loader
```

Also you can clone the repository or [download the zip file](https://github.com/raphaelfabeni/css-loader/archive/master.zip) and get main *CSS* file that it's located in: `dist/css-loader.css`.

## Setup

Add the CSS file in your project and add the link to the file:

```html
<link rel="stylesheet" href="path/to/css-loader.css">
```

Select the loader and add the HTML corresponding to it, To show the loader, you need to add the helper css class `is-active`. And to hide the loader, it's just follow the inverse, removing the css helper from the loader. You can do it with JavaScript.

```html
<!-- Loader -->
<div class="loader loader-default"></div>

<!-- Loader active -->
<div class="loader loader-default is-active"></div>
```

## Examples

### Default

```html
<div class="loader loader-default is-active"></div>
```

![loader](https://cloud.githubusercontent.com/assets/1345662/19313531/2c715f18-906d-11e6-856a-17ca264112de.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-default) :metal:

#### Variations

**data-text**: it's to add a _Loading_ text into the loader. Just add the `data-text` attribute.

```html
<div class="loader loader-default is-active" data-text></div>
```

![loader-data-text](https://cloud.githubusercontent.com/assets/1345662/19313794/1fdf0ce0-906e-11e6-8a9f-39d2421a41d6.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-default-text) :metal:

It's also possible to change the text, just passing a value to the attribute `data-text`.

```html
<div class="loader loader-default is-active" data-text="Custom text"></div>
```

![loader-data-text-custom](https://cloud.githubusercontent.com/assets/1345662/19313797/21e3fb22-906e-11e6-8f0a-11cc9c0fb8d2.gif)

**blink**: passing the `blink` attribute, you can add a simple _fade_ animation to the text loader

```html
<div class="loader loader-default is-active" data-text blink></div>
```

![loader-blink](https://cloud.githubusercontent.com/assets/1345662/19313798/25fa2830-906e-11e6-88d2-2f165a68cb80.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-default-blink) :metal:

**half**: a _half_ loader.

![loader-half](https://cloud.githubusercontent.com/assets/1345662/19418371/55ae80cc-93a1-11e6-9273-22955e62a6a4.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-default-half) :metal:

They variations _half_, _data-text_ and _blink_ work together. 😄

### Double

```html
<div class="loader loader-double is-active"></div>
```

![loader-double](https://cloud.githubusercontent.com/assets/1345662/19314508/c2279a06-9070-11e6-8079-4fa82b5f2610.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-double) :metal:

### Bar

```html
<div class="loader loader-bar is-active"></div>
```

![loader-bar](https://cloud.githubusercontent.com/assets/1345662/19314685/6d719056-9071-11e6-88c8-2c3750ca0198.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-bar) :metal:

#### Variations

Like the `loader` example, it's also possible pass the `data-text` and `blink` attributes.

```html
<div class="loader loader-bar is-active" data-text></div>
<!-- -->
<div class="loader loader-bar is-active" data-text="Custom text"></div>
<!-- -->
<div class="loader loader-bar is-active" data-text blink></div>
```

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-bar-text) :metal:

**rounded**: passing the `rounded` attribute, it's possible to add a simple `border-radius` to the loader.

![loader-bar-rounded](https://cloud.githubusercontent.com/assets/1345662/19315031/ab850700-9072-11e6-9cd4-9fe899f05a10.gif)

```html
<div class="loader loader-bar is-active" data-text rounded></div>
```

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-bar-rounded) :metal:

### Border

![loader-border](https://cloud.githubusercontent.com/assets/1345662/19314686/6d733622-9071-11e6-8167-a55e6c16a02f.gif)

```html
<div class="loader loader-border is-active"></div>
```

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-border) :metal:

#### Variations

Like the `loader` example, it's also possible pass the `data-text` and `blink` attributes.

```html
<div class="loader loader-border is-active" data-text></div>
<!-- -->
<div class="loader loader-border is-active" data-text="Custom text"></div>
<!-- -->
<div class="loader loader-border is-active" data-text blink></div>
```

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-border-text) :metal:

### Ball

```html
<div class="loader loader-ball is-active"></div>
```

![loader-ball](https://cloud.githubusercontent.com/assets/1345662/19314687/6d771ff8-9071-11e6-8839-713066f11056.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-ball) :metal:

#### Variations

*shadow*: a version of the ball with inset shadow.

![loader-ball-shadow](https://cloud.githubusercontent.com/assets/1345662/19502619/06f1c906-958d-11e6-87c9-d64b13688485.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-ball-shadow) :metal:

### Smartphone

```html
<div class="loader loader-smartphone is-active"></div>
```

![loader-smartphone-empty](https://cloud.githubusercontent.com/assets/1345662/19544262/83cd4b42-965c-11e6-9238-91a48f0d5cf5.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-smartphone) :metal:

#### Variations

*w/ screen text*: it's possible to pass an attribute to loader and show a simple text inside the screen. Like the others one, if we only pass the attribute, a default _loading_ text shows; but you can pass a custom text. Just remember that can't be a big word (our smartphone screen is small).

```html
<!-- default loading text -->
<div class="loader loader-smartphone is-active" data-screen></div>

<!-- custom text -->
<div class="loader loader-smartphone is-active" data-screen="hello"></div>
```

![loader-smartphone](https://cloud.githubusercontent.com/assets/1345662/19544263/83ec08a2-965c-11e6-99f3-fea1896c0191.gif)

[See it](http://raphaelfabeni.com.br/css-loader/#/loader-smartphone-text) :metal:

## Contributing

1. Clone this repository.
2. `npm install` and `gulp`
3. Open => `http://localhost:300`
4. Make your magic contribution.
5. Open a _PR_ with a new branch describing your changes. <o/

## Browser Support

All examples use CSS _animation_ which is supported by [most current browsers](http://caniuse.com/#search=animation).

| <img src="https://github.com/alrra/browser-logos/blob/master/chrome/chrome_128x128.png?raw=true" width="48px" height="48px" alt="Chrome logo"> | <img src="https://github.com/alrra/browser-logos/blob/master/firefox/firefox_128x128.png?raw=true" width="48px" height="48px" alt="Firefox logo"> | <img src="https://github.com/alrra/browser-logos/blob/master/internet-explorer/internet-explorer_128x128.png?raw=true" width="48px" height="48px" alt="Internet Explorer logo"> | <img src="https://github.com/alrra/browser-logos/blob/master/opera/opera_128x128.png?raw=true" width="48px" height="48px" alt="Opera logo"> | <img src="https://github.com/alrra/browser-logos/blob/master/safari/safari_128x128.png?raw=true" width="48px" height="48px" alt="Safari logo"> | <img src="https://raw.githubusercontent.com/alrra/browser-logos/master/android/android_128x128.png" width="48px" height="48px" alt="Android Browser Logo" >
|:---:|:---:|:---:|:---:|:---:|:---:|
| 43+ ✔ | 16+ ✔ | 10+ ✔ | 30+ ✔ | 9+ ✔ | 5.2+ ✔

Based on _Can i Use_. One thing to note is the CSS file has no browsers prefixes, but you can easily add and increase the support of the browsers.

## Licence

[MIT License](https://raphaelfabeni.mit-license.org/) © Raphael Fabeni

