


```[![Build status](https://updatelater/iron-movable-container.svg?branch=master)](https://updatelater/iron-movable-container)```

```_[Demo and API docs](https://thislinkwontwork)_```

# This project was modified from the existing iron-swipeable-container project

to install:
`bower install --save krumware/iron-movable-container`

Feel free to contribute!

Plans for this project:
  - Handle parent element bounds
  - Provide "sticky/snap"
  - Allow resizing
  - Develop paper/material component

##&lt;iron-movable-container&gt;

`<iron-movable-container>` is a container that allows any of its nested
children (native or custom elements) to be anchor elements, that can be dragged to move the element.

Example:

```html
    <style>
      .toolbar {
        @apply(layout-fixed-top);
        @apply(layout-flex);
        height:20px;
        background-color:green;
      }
    </style>
    <iron-movable-container>
      <div class="drag-anchor toolbar">I can be dragged</div>
      <paper-card heading="I'm just tagging along"></paper-card>
    </iron-movable-container>
```

Alternatively, to disable the drag, used the `disabled` attribute.

```html
    <style>
      .toolbar {
        @apply(layout-fixed-top);
        @apply(layout-flex);
        height:20px;
        background-color:green;
      }
    </style>
    <iron-movable-container disabled>
      <div class="drag-anchor toolbar">I can be dragged</div>
      <paper-card heading="I'm just tagging along"></paper-card>
    </iron-movable-container>
```

It is a good idea to disable text selection on any of the children that you
want to be draggable:

```css
.drag-anchor {
  -moz-user-select: none;
  -ms-user-select: none;
  -webkit-user-select: none;
  user-select: none;
  cursor: default;
}
```


