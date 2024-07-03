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