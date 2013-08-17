#Magic Header (JQuery plugin)#

What is this ?
--------------

*This JQuery plugin is an Open-source plugin for more magic in your headers*

> ### [DEMO HERE !](http://remidelhaye.github.io/MagicHeader)


How it works ?
--------------

First, I use JQuerys powerness. This is a very simple, light, and easy to use plugin.

##### HTML :

```html

<!-- A simple <header> tag works very well -->

<header>
    Scroll to show/hide your header!
</header>

```

##### Javascript :

```javascript

// Simple use

$('header').magicheader();

// With options

$('header').magicheader({
    delay: 4000,
    minScroll: 0,
    detachedClass: 'fixed',
    hiddenClass: 'hidden'
});

```

##### CSS :

```css

header {
  width: 100%;
  height: 100%;
  max-height: 50px;
  position: absolute;
  top: 0;
  overflow: hidden;
  z-index: 100;
  -webkit-transform: translate3d(0, 0, 0);
  -webkit-transition-duration: .2s;
  -webkit-transition-property: opacity,-webkit-transform,background;
  -webkit-transition-timing-function: ease-in-out;
  -webkit-backface-visibility: hidden;
  -webkit-perspective: 1000;
  left: 0px;
  right: 0px;
  text-align: center;
  color: white;
  line-height: 50px;
}
header.hidden {
  opacity: 0;
  -webkit-transition-duration: .25s;
  -webkit-transform: translate3d(0, -50px, 0);
}
header.fixed {
  background: white;
  color: #4183c4;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
  position: fixed;
  opacity: 1;
}

```

Contributors
------------

 * Creator : [@RemiDelhaye](https://github.com/RemiDelhaye) ([http://remidelhaye.fr](http://remidelhaye.fr))
