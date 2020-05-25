# Responsiveness with CSS
Result of <b>RocketSeat's Masterclass # 08</b>, in which the subject of responsiveness using CSS is addressed.

## :page_with_curl: Project
The goal of the masterclass is to make a fixed page responsive, adjusting all elements to the correct size according to the screen size of each device.

## :clipboard: Topics covered

- ### ***CSS Units***

Units  | Meaning
--- | ---
`px`  | Pixel
`%` | Percentage
`auto` | Automatic
`vh` | Viewport Height
`vw` | Viewport Width
`1px` | 0.75pt
`em` | Relative to the font-size of the element
`rem` | Relative to font-size of the root element
 
- ### ***CSS Media Queries*** 

#### HTML
 ```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

#### CSS
```css
@media (max-width: 320px) {
  #form h3 {
    font-size: 2rem;
  }
}
```
- ### ***HTML Media Attributes***

It is possible to use the attribute `media` in the `<link>` tag of HTML, when importing a CSS file, using the properties in the same way that `@ media` is used in CSS.

```html
<link 
    rel="stylesheet"
    href="responsive.css" 
    media="screen and (max-width: 768px)"
/>

<link rel="stylesheet" href="print.css" media="print">
```

- ### ***Images***

Using the `<picture>` tag makes the images responsive.

```html
<picture class="image" alt="Imagem">
    <source media="(min-width: 768px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/maxresdefault.jpg">
    <source media="(min-width: 320px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg">
    <source media="(min-width: 10px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/mqdefault.jpg">

    <img 
        src="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg" 
        alt="Imagem" />
</picture>
```
