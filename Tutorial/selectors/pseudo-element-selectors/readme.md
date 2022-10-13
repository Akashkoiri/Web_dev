## Pseudo_element_selectors

### [1] ::before & ::after

```css
p::before,
p::after {
    content: ''; /* Very important */
    display: block;
    background-color: red;
    height: 10px;
}
```

### [2] add images & icons

```css
p::before {
    content: url(//unsplash.it/50/50);
}
```

### [2] add custom stylish quotes

```css
p::before {
    content: open-quote;
}
```