[回到目录](../../README.md)

<hr>
<hr>
<br>

# | Flexbox |

## [02:15:00] Flex

大 layout 用 grid system
内部 elment 用 flex

Flex 练习平台:

- [Flexbox Playground](https://flexbox.tech/)

参考链接：

- [W3School Flexbox](https://www.w3schools.com/csS/css3_flexbox.asp)
- [MDN Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
- [CSS Trick - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## 常用 Flex Properties

### [02:32:00] Flex 方向

```css
.flex-box {
  display: flex;
  flex-direction: row | row-reverse | column | column-reverse;
}
```

### [02:34:00] Flex Warp

```css
.flex-box {
  display: flex;
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

### [02:36:00] Flex 对齐

#### 横向对齐（Horizontal Alignment）

```css
.flex-box {
  display: flex;
  justify-content: flex-start | flex-end | center | space-between | space-around
    | space-evenly;
}
```

![Flex justify-content sample](./note-assets/flex-justify-content.svg)

#### 纵向对齐（Vertical Alignment）

```css
.flex-box {
  display: flex;
  align-items: flex-start | flex-end | center | stretch | baseline;
}
```

![Flex justify-content sample](./note-assets/flex-align-items.svg)

_[02:50:00 - Class break]_

<br>
<hr>
<hr>

## _[ Switch to [Bootstrap](03_bootstrap.md) ]_
