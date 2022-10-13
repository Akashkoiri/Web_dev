### How to make blured glass ?

```css
body {
	background: #161623;
}
.container .card {
	background: rgba(255, 255, 255, .05);
	box-shadow: 0 15px 35px rgba(0, 0, 0, .2);
    	backdrop-filter: blur(10px);
}
```