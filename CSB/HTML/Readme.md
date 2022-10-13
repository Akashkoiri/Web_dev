# HTML Tutorial

---

## Tags:-

### <h1> - <h6>
### <p>
### <br>
### <hr>
### <b>
### <i>
### <sup>
### <sub>
### <small>
### <a>

### HTML Entitis:

```html
> => &lt
< => &gt
```

## Media Tags:-

### <video> 
* src="videos/video.mp4" 
* width="400" height="600" 
* autoplay 
* controls
* loop 
* muted
* poster="thumbnail.jpg"

### <iframe>
<!-- 1. Go to youtube
     2. click share
     3. Embed video
     4. copy & paste the iframe code in the html file  -->

* src="https://www.youtube.com/embed/JUJDMWS1-dY"
* frameborder="1"
* allow="accelerometer autoplay"
* allowfullscreen


## Table Tag:-

* Table = <table>

@ Attributes:-
* border="1"

* Table-Row = <tr>

* Table-heading = <th>
* Table-data = <td>

@ Attributes:-
* rowspan="2"
* colspan="4"

### Table Structure / Grouping sections of a table

* Table-heading-section = <thead>
* Table-body-section = <tbody>
* Table-footer-section = <tfoot>

<!-- colspan use karte time <th> ka use kare jisse content middle me aa jata hi -->


## Form:-

* Form-Tag = <form></form>

@ Attributes:-
    * method
    * action

* input Element = <input>

@ Attributes:-
    * type="text/passowrd/radio/checkbox/file/submit/reset/image
    * name="anyname" <!--Name is must for backend data processing>
    * value="predefine-value"

* textarea = <textarea></textarea>

@ Attributes:-
    * cols="80"
    * Rows="10"


* Select box = <select></select>

* Options = <option></option>

@ Attributes:-
    * value="Delhi"


* Create a box and wrapp = <fieldset></fieldset>

* Give a name to the field = <legend></legend>

* We can specify a cell is required = <input required>


### How to make the footer stick to the bottom?

```css
body {
    height: 100vh;
}
footer {
    position: sticky;
    top: 100%;
}

```