# HTML & CSS DAY 4

- google font
- display flex
- display grid
- nav menu

### Google Fonts

import font in html ```head```
```html 
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Thai:wght@100..900&family=Prompt:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
```
use font in css ```style```
```css
.container {
     font-family: "Noto Sans Thai", sans-serif;
}
```

- [Google Fonts](https://fonts.google.com/)

### Display flex
css
```css
.flex {
    display: flex;
    margin-bottom: 1rem;
}

.flex-start {
    justify-content: flex-start
}

.flex-end {
    justify-content: flex-end
}

.center {
    justify-content: center;
}

.space-between {
    justify-content: space-between;
}

.space-around {
    justify-content: space-around;
}

.space-evenly {
    justify-content: space-evenly;
}
```

html
```html
<div class="flex space-evenly">
    <div class="item red"></div>
    <div class="item green"></div>
    <div class="item blue"></div>
</div>
```


### Dissplay grid
css
```css
.grid {
    display: grid;
}

.grid-cols-3 {
    /* 1fr 1fr 1fr */
    grid-template-columns: repeat(3, minmax(0, 1fr));
}

.layout {
    grid-template-columns: repeat(4, minmax(0, 1fr));
}

.item1 {
    background-color: orange;
    padding: 10px;
    text-align: center;
    grid-column: span 4 / span 4;
}
.item2 {
    background-color: blue;
    padding: 10px;
    text-align: center;
    grid-column: span 2 / span 2;
}
.item3 {
    background-color: white;
    padding: 10px;
    text-align: center;
}
.item4 {
    background-color: red;
    padding: 10px;
    text-align: center;
}
.item5 {
    background-color: green;
    padding: 10px;
    text-align: center;
    grid-column: span 4 / span 4;
}
```
html
```html
<!-- Display Grid -->
        <div class="grid grid-cols-3" style="margin-bottom: 1rem;">
            <div class="item red"></div>
            <div class="item green"></div>
            <div class="item blue"></div>
            <div class="item red"></div>
            <div class="item green"></div>
            <div class="item blue"></div>
        </div>
        <!-- Layout -->
        <div class="grid layout">
            <div class="item1">
                header
            </div>
            <div class="item2">
                main
            </div>
            <div class="item3">
                empty
            </div>
            <div class="item4">
                sidebar
            </div>
            <div class="item5">
                footer
            </div>
        </div>
```

### Nav menu
- tag nav
- link
- css display flex

1. html tag nav 
html
```html
<nav></nav>
```
2. list item
html
```html
<nav>
    <ul>
        <li>
            <a href="#">Home</a>
        </li>
        <li>
            <a href="#">About</a>
        </li>
        <li>
            <a href="#">Contact</a>
        </li>
    </ul>
</nav>
```

3. custom list item
css
```css
nav {
    padding: 10px;
}

ul {
    display: flex;
    justify-content: center;
    flex-direction: row;
    list-style-type: none; 
}

ul li {
    padding: 10px 20px;
    text-align: center;
}
```