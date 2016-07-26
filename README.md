
<!---

This README is automatically generated from the comments in these files:
iron-movable-container.html

Edit those files, and our readme bot will duplicate them over here!
Edit this file, and the bot will squash your changes :)

The bot does some handling of markdown. Please file a bug if it does the wrong
thing! https://github.com/PolymerLabs/tedium/issues

-->

```[![Build status](https://travis-ci.org/PolymerElements/iron-movable-container.svg?branch=master)](https://travis-ci.org/PolymerElements/iron-movable-container)```

_[Demo and API docs](https://elements.polymer-project.org/elements/iron-movable-container)_


##&lt;iron-movable-container&gt;

`<iron-movable-container>` is a container that allows any of its nested
children (native or custom elements) to be swiped away. By default it supports
a curved or horizontal transition, but the transition duration and properties
can be customized.

Example:

```html
<iron-movable-container>
  <div>I can be swiped</div>
  <paper-card heading="Me too!"></paper-card>
</iron-movable-container>
```

To disable swiping on individual children, you must give them the `.disable-swipe`
class. Alternatively, to disable swiping on the whole container, you can use its
`disable-swipe` attribute:

```html
<iron-movable-container>
  <div class="disable-swipe">I cannot be swiped be swiped</div>
  <paper-card heading="But I can!"></paper-card>
</iron-movable-container>

<iron-movable-container disable-swipe>
  <div>I cannot be swiped</div>
  <paper-card heading="Me neither :("></paper-card>
</iron-movable-container>
```

It is a good idea to disable text selection on any of the children that you
want to be swiped:

```css
.swipe {
  -moz-user-select: none;
  -ms-user-select: none;
  -webkit-user-select: none;
  user-select: none;
  cursor: default;
}
```


