## Flex Box

### [1] How to use Flex Box?

```css
.container {
    display: flex;
}
```

### [2] How to change Flex Direction?

```css
.container {
    display: flex;
    flex-direction: row/column-reverse
}
```

### [3] How to align child elements position row-wise?

```css
.container {
    display: flex;
    justify-content: center/right, space-between,-around,-evenly
}
```

### [4] How to align child elements position column-wise?

```css
.container {
    display: flex;
    align-items: start/center/end;
}
```

### [5] Diffrence Between align-content & align-items?

```css
.container {
    display: flex;
    flex-wrap: wrap;
    /* Both of them are used to align multiline child eliments/After they got wrap by resizing window we can use them*/

    /* align-content will not give an empty space between lines after wrap */
    align-content: flex-start/flex-end,space-between/space-around;
    /* align-items will give an empty space between lines after wrap */

    align-items: flex-start/center/flex-end;
}
```

### [6] Diffrence between align-items & align-self?

```css
/* align-items are write inside the container elements & applied to all child elements*/
.conteiner {
    align-items: center;
}
/* align-self are write inside the child elements & applied to only that child element*/
.child1 {
    align-self: flex-end;
}
```

### [7] How to change order of elements using css without chenging it from html file?

```css
.conteiner {
    align-items: center;
}
.child1 {
    align-self: flex-end;
    order: 3;
}
.child2 {
    align-self: flex-end;
    order: 1;
}
.child3 {
    align-self: flex-end;
    order: 2;
}
```

### [8] How to use flex-grow,flex-shrink & flex-basis in oneline?

```css
div {
    /* flex: grow shrink basis */
    flex: 1 0 5px
    /* basis = sets the normal width of the element */
}
```
### [9] How to stop overflow?

```css
.container {
    height: 200px;
    width: 200px;
    border: 1px solid black;
    
}
.child {
    height: 80px;
    width: 80px;
    background-color: red;
    border: 1px solid black;
    margin: 5px;
}
```