# Shell
A light, modern, 12-column, css grid layout. Less than 200 lines of code!!

### About
Shell uses css-grid to make your website's grid layouts easy to read and easy to make. No longer will you need float things, use flex boxes, or use endless amount of nested divs. What you write is what you get.

# Quick Setup
- Paste the CDN in your head tag. (I'm broke and can't afford services like MaxCDN, so this will probably be slow)
```html
<link rel="stylesheet" href="https://sniddl.com/cdn/grid.min.css">
```

# Setup
- Download the files you want.
- Add one of the files to your css folder.
- Link the file with HTML
```html
<link rel="stylesheet" href="/css/grid.min.css">
```
- Get coding fast!

# Syntax
Define the grid. You can have multiple grids. Or add rows inside your grid.
```html
<div class="grid">
  <div class="row"></div>
</div>
```

Add your content.
```html
<div class="grid">
  <div class="mydiv">...</div>
</div>
```

Make it go where you want it to go. Just add 2 classes, the starting point and the ending point.
The column numbers range from 1-12.

||column|class|definition|
|---|---|---|---|
|start|1|s1|start the element at the first column
|end|4|e4|end the element at the fourth column

```html
<div class="grid">
  <div class="mydiv s1 e4">...</div>
</div>
```

There you go. Easy as 123. 
Now if want to add responsiveness, just tell it where you want it to become full width.

||classes|pixel size|
|---|---|---|
|small|small, sm|576px|
|medium|medium, md|768px|
|large|large, lg|992px|
|extra large|xlarge, xl| 1200px|

The following example will start at column 4 and will end at column 6. Then when the website is the size of a phone, it will take up the full page.
```html
<div class="grid">
  <div class="mydiv s4 e6 small">...</div>
</div>
```
Then if you want to remove the gap between the items, add the `no-gap` class on the grid.
```html
<div class="grid no-gap">
  <div class="mydiv s4 e6 small">...</div>
</div>
```

Here is an example on jsfiddle
https://jsfiddle.net/zebthewizard/dnmvuszy/3/
