#

### How to use transition to animate stuffs?

```html
<div class="parent">
        <div class="child">
        </div>
    </div>
```
```css
.child {
/* This is must use for smoothness on the element that has animation */
    transition: 1s ease-in-out 1s;
/* transition: smooth type delay */
}

.parent:hover .child {
    /* These are the animations */
    background: greenyellow;
    transform: translateX(100%);
}
```

### How to use @keyframes & animation?

```css
.parent:hover .child {
    /* 1. anime is the name of keyframe*/
    animation: anime 1s ease-in-out;
}

@keyframes anime {
    /* These  are the position where the box will go through the animation */
    0% {
        transform: translateX(0) ;
    }
    33% {
        transform: translateY(100%);
    }
    66% {
        transform:  translateX(100%) translateY(100%);
    }
    100% {
        transform: translateX(100%) ;
    }
}
```

### Another way to animate?

```css
@keyframes {
    from[]
    to[]
}
```

### How to make the keyframes stay on 100% even after the animation ended?

```css
/* Just add the forward value */
.parent:hover .child {
    animation: anime 1s forwards;
}
```

### How to set a diffrent styling at the time of delay?

```css
.parent:hover .child {
    animation: anime 1s backwards 2s;
}
/* Change the 0% keyframe */
```

### How to make the animation repeate diffrent times?

```css
/* The animation will go for 2 times */
.parent:hover .child {
    animation: anime 1s ease-in-out 2s 2;
}

/* The animation will go for infinite times */
.parent:hover .child {
    animation: anime 1s ease-in-out 2s infinite;
}
```

### How to set animation direction?

```css
.parent:hover .child {
    animation: anime 1s ease-in-out infinite alternate;
}
```
