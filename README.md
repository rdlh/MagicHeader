#Magic Header JQuery#

What is this ?
--------------

*This JQuery plugin is an Open-source plugin for more magic in your headers*

> ### [DEMO HERE !](http://remidelhaye.github.io/MagicHeader)


How it works ?
--------------

First, this plugin use JQuery powerness. This is a very simple, light, and easy to use plugin.

##### HTML :

```html


<button id="show-menu">Show/Hide Menu</button>

<nav class="my-responsive-menu" id="menu-left">
  <h3>Menu</h3>
  <a href="#">1st link</a>
  <a href="#">2nd link</a>
  <a href="#">3rd link</a>
</nav>

```

##### Javascript :

```javascript


document.getElementById( 'show-menu' ).onclick = function() {
  classie.toggle( this, 'active' );
  classie.toggle( document.getElementById( 'menu-left' ), '.my-responsive-menu-open' );
};

```

##### CSS :

```css


.my-responsive-menu {
  position: fixed;
  width: 240px;
  height: 100%;
  top: 0;
  z-index: 1000;
  left: -240px;
}

.my-responsive-menu-open {
  left: 0px;
}

```

Contributors
------------

 * [@RemiDelhaye](https://github.com/RemiDelhaye) ([http://remidelhaye.fr](http://remidelhaye.fr))

Good issues
-----------

 * [@Tiste](https://github.com/tiste) ([http://tiste.io](http://tiste.io)) - [Issue #1](https://github.com/RemiDelhaye/MobileMenu/issues/1)
