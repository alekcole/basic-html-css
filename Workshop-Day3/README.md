# HTML & CSS DAY 3

- link css file
- box sizing
- box model
    - margin
    - pending
    - border
- max width
- display

### link css file
เพิ่ม ไฟล์ css ไว้ใน project และ เรียกใช้ file css
```html
...
<link rel="stylesheet" href="css/style.css">
...
```
### box sizing
```css
* {
    box-sizing: border-box;
}
```
### box model

- margin
- padding
- border 
- border-radius

```css
.margin {
    margin: 10px;
    /* แยกตามมุม */
    margin-top: 10px;
    margin-bottom: 10px;
    margin-left: 10px;
    margin-right: 10px;
    /* หรือ */
    /* top left bottom right */
    margin: 5px 10px 5px 10px;
}

.padding {
    padding: 10px;
    /* แยกตามมุม */
    padding-top: 10px;
    padding-bottom: 10px;
    padding-left: 10px;
    padding-right: 10px; 
    /* หรือ */
    /* top left bottom right */
    padding: 5px 10px 5px 10px;
}

.border {
    border: 1px solid #fff;
    /* widht style color */
    border-width: 1px;
    border-style: solid;
    border-color: #fff;
}

.border-radius {
    border-radius: 10px;
     /* แยกตามมุม */
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
      /* หรือ */
    /* top left bottom right */
    border-radius: 5px 10px 5px 10px;
}
```

### max width

```css
div {
   max-width: 300px;
}
```

max-width + margin
```css
div {
   max-width: 300px;
   margin: 0 auto;
}
```

### Display

block element
```html
<p>block element</p>
<p>block element</p>
```

inline element
```html
<span>inline element</span>
<span>inline element</span>
```

เปลี่ยน จาก inline เป็น block element
```css
span {
    display: block;
}
```


เปลี่ยน จาก block เป็น inline element
```css
span {
    display: inline;
}
```

display รูปแบบอื่นๆ
```css
div {
    display: block;
    display: inline;
    display: none;
    display: flex;
    display: grid;
    visibility: hidden
}
```