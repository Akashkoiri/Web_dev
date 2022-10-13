## Position:

### [1] Relative:

```html
<div class="outer">
    <div class="inner1"></div>
</div>
```
```css
.outer {
    height: 400px;
    width: 400px;
    margin: auto;
    border: 2px solid black;
}

.inner {
    height: 150px;
    width: 150px;
    background-color: red;
    /* If we set position to relative then we can access top/bottom/left/right */
    position: relative;
    /* It tells that how far we need our element from it's original position & from wich side*/
    right: 10px;
}
```

### [2] Absolute:

```html
<div class="outer">
    <div class="inner1"></div>
</div>
```
```css
.outer {
    height: 400px;
    width: 400px;
    margin: auto;
    border: 2px solid black;
}

.inner {
    height: 150px;
    width: 150px;
    background-color: red;
    /* If we set position to absolute then we can access top/bottom/left/right */
    position: absolute;
    /* It tells that how far we need our element according to the body & from wich side*/
    bottom: 10px;
}
```

#### Two elements position

<!-- Absolute child always follow the relative perent, If there is no relative perent then it will follow the body tag -->

```css
.outer1 {
    height: 400px;
    width: 400px;
    margin: auto;
    border: 2px solid black;
    position: relative;
}

.inner1 {
    background-color: red;
    position: absolute;
    top: 10px;
    right: 10px;
}
```

### [3] Fixed:

<!-- Fixed is behave like absolute but wherever it placed it will going to fix it's position. even after scrolling-down it will not going to move itself from that position in window -->

```css
.outer1 {
    height: 400px;
    width: 400px;
    margin: auto;
    border: 2px solid black;
}

.inner1 {
    background-color: red;
    position: fixed;
    top: 10px;
    right: 10px;
}
```

### [4] sticky:

<!-- sticky is used to create navigation bars. when we scroll-down & Whenever it touches the end of the window it will act like fixed position element -->

```css
.outer1 {
    height: 400px;
    width: 400px;
    margin: auto;
    border: 2px solid black;
}

.inner1 {
    background-color: red;
    position: sticky;
    top: 1px;
```

### [#] How to center a content even after giving position?

```css
.box {
    height: 100px;
    width: 100px;
    position: relative;
}

.child {
    height: 40px;
    width: 40px;
    background: red;
    position: absolute;

    margin: auto;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
}
```