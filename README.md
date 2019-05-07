# Share Buttons [![npm](https://img.shields.io/npm/v/share-buttons.svg)](https://www.npmjs.com/package/share-buttons) ![license](https://img.shields.io/github/license/wcoder/share-buttons.svg)

Simple, powerful, customizable and lightweight social buttons for your site.

## [Demo](https://alexander-logachev.github.io/share.buttons/)

## Browser support

* Google Chrome
* Mozilla Firefox 3.5+
* Opera 10+
* Safari 3.2+
* IE 8+
* Android
* iOS

## Install

NPM:

```sh
npm i share-buttons
```

##Usage

AMD module:

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.6/require.min.js"></script>
<script src="../src/share-buttons.js"></script>
<script>
    require(['ShareButtons'], function (ShareButtons) {
         new ShareButtons();
    });
</script>
```

Browser globals:

```
<script src="../src/share-buttons.js"></script>
<script>
    new ShareButtons();
</script>
```

Paste this html on the page:

``` html
<div class="share-btn">
    <a class="btn-vk" data-id="vk">VK</a>
    <a class="btn-facebook" data-id="fb">Facebook</a>
    <a class="btn-twitter" data-id="tw">Twitter</a>
    <a class="btn-telegram" data-id="tg">Telegram</a>
    <a class="btn-mail" data-id="mail">EMail</a>
</div>
```

Added styles:

``` css
.share-btn > a {
    border: 1px solid #ccc;
    padding: 5px;
    font-size: 12px;
    font-family: Verdana, Arial;
}
.share-btn > a:hover {
    cursor: pointer;
}
```

Options:

Parameters        | Description
---------------|---------------
elementID      | id or class of element (by default `.share-btn`)
erroMsgFunc    | callback on error event

Example:

```
new ShareButtons({elementID: '.js-share-buttons' ,erroMsgFunc: function (msg) {
    console.log(msg);
}});
``` 

## Share via

Network        | `data-id`
---------------|---------------
Facebook       | fb
VK             | vk
Twitter        | tw
Telegram       | tg
Pocket         | pk
Reddit         | re
Evernote       | ev
LinkedIn       | in
Pinterest      | pi
Skype          | sk
WhatsApp       | wa
Viber          | viber
Odnoklassniki  | ok
Tumblr         | tu
Hacker News    | hn
Xing           | xi
EMail          | mail
Print          | print
Print          | print
Мой мир        | my
Livejournal    | lj
Add to favorite   | fav

## Customizing

Custom 'url', 'title', 'description':

``` html
<div class="share-btn" data-url="https://..." data-title="..." data-desc="...">
    <a class="btn-vk" data-id="vk">VK</a>
    <a class="btn-facebook" data-id="fb">Facebook</a>
    <a class="btn-twitter" data-id="tw">Twitter</a>
    <a class="btn-telegram" data-id="tg">Telegram</a>
    <a class="btn-mail" data-id="mail">EMail</a>
</div>
```

Styles - full customization.

## Examples

If your using [Font-Awesome](https://github.com/FortAwesome/Font-Awesome):

```html
<div class="share-btn" data-url="https://..." data-title="..." data-desc="...">
    <a class="btn-vk" data-id="vk"><i class="fab fa-vk"></i> VK</a>
    <a class="btn-facebook" data-id="fb"><i class="fab fa-facebook-square"></i> Facebook</a>
    <a class="btn-twitter" data-id="tw"><i class="fab fa-twitter"></i> Twitter</a>
    <a class="btn-telegram" data-id="tg"><i class="fab fa-telegram"></i> Telegram</a>
    <a class="btn-mail" data-id="mail"><i class="fas fa-at"></i> EMail</a>
</div>
```

----

&copy; 2015 - 2019 Alexander Logachev
