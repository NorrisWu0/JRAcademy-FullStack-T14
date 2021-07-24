[回到目录](../../README.md)

<hr>
<hr>
<br>

# | Responsive Web Design |

面试很大几率会考 responsive web design strategies.

## [00:38:00] What is Responsive Web Design

must known, even for developers!

Responsinve

![Responsive Design Sample](/course-materials/l03_css_scss/note-assets/resize.gif)

## [00:44:30] How to make responsive web design

use @media queries.
<br>

---

### **静态设置 - Static Setting**

#### 使用 CSS @media queries

```css
/* 窗口大小600px以内 */
@media screen and (max-width: 600px) {
}

/* 窗口大小至少900px */
@media screen and (min-width: 900px) {
}
```

<br>

#### 使用 viewport

viewport 可以通过

```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
```

屏幕大小和手机分辨率不成正比，举个例子为，电脑屏幕尺寸可能为 27 寸，但他的分辨率可能是 1920px \* 1080px。而手机虽然屏幕大小只有 6 寸，但它的分辨率可能是 2280px \* 1080px;

<br>

#### 使用 breakpoint

<br>

---

### [000:58:00] **动态设置 - Dynamic Setting**

#### External Grid System Libraries

参考链接：

- [Bootstrap - Grid System](https://getbootstrap.com/docs/4.0/layout/grid/)

#### CSS Grid

参考链接：

- [W3School - CSS Grid Layout](https://www.w3schools.com/css/css_grid.asp)
- [MDN - CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
- [CSS Trick - Complete Guide to CSS](https://css-tricks.com/snippets/css/complete-guide-grid/)

_[01:08:00 - class break]_

<br>
<hr>
<hr>

## _[Switch to [Sass](03_scss.md)]_
