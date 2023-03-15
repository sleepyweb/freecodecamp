# Set of Colored Markers

## Notes:

`rgba`  It’s for red, green, blue and alpha. We can put the value between 0 to 255 for r,g and b or 0 to 100%. Alpha is for the opacity, the range is 0.0(fully transaparent) to 1.0(fully opaque).

`border`  It’s to set border for the content. Constituent properties are `border-color` , `border-style`, `border-width` 

`border-left` , `border-right` , `border-top` , `border-bottom` To set borders for left, right, top and bottom. 

`linear-gradient` It creates an image, consisting of two or more colors transition along straight line.

`box-shadow` It adds shadow effects around content’s frame.

Different Color Notation:

`rgba`, `hsla`, hexcodes

![HEX Color Code](/responsiveWebDesign/SetofColoredMarkers/notes_img/img_1.png)

---

## Code Snipets:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colored Markers</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <h1>CSS Color Markers</h1>
    <div class="container">
      <div class="marker red">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker green">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker blue">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
    </div>
  </body>
</html>
```

```css
h1 {
    text-align: center;
}
  
.container {
    background-color: rgb(255, 255, 255);
    padding: 10px 0;
}
  
.marker {
    width: 200px;
    height: 25px;
    margin: 10px auto;
}
  
.cap {
    width: 60px;
    height: 25px;
}
  
.sleeve {
    width: 110px;
    height: 25px;
    background-color: rgba(255, 255, 255, 0.5);
    border-left: 10px double rgba(0, 0, 0, 0.75);
}
  
.cap, .sleeve {
    display: inline-block;
}
  
.red {
    background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
    box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
}
  
.green {
    background: linear-gradient(#55680D, #71F53E, #116C31);
    box-shadow: 0 0 20px 0 #3B7E20CC;
}
  
.blue {
    background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
    box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);
  }
```
