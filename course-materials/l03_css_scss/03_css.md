[回到目录](../../README.md)

<hr>
<hr>
<br>

# | CSS - Cascading Style Sheets - Part 2 |

## [00:11:00] Card

card 是十分常见的 web element，通常都以 component 的形式出现。但现阶段的学习还未涉及 component，所以我们用 plain html 编写 card element。

## [00:14:30] Styling Guide

#### Style from top to bottom

浏览器在读取 css 文件时会从上往下读取，如果在同一个文件冲出现重复的 class selector，那么浏览器会优先采用后者的 class selector properties。

#### Style from different source

使用外部 css 文件，例如[normalize.css]().

优先级

1.
2. User Stylesheet
3. Default Stylesheet

## [00:20:00] CSS Reset - 面试点

[CSS tools: Reset CSS - by Eric Meyer](https://meyerweb.com/eric/tools/css/reset/)

不用 universal selector 的好处在于，Reset CSS 能 explicitly reset 特定元素。这样开发能更精准的掌控被重置的元素。

## [00:22:40 - 00:32:30] CSS Selector Specificity - 优先级

|  低  |   高   |
| :--: | :----: |
| Left | Right  |
| Top  | Bottom |

[参考文件](https://github.com/NorrisWu0/JRAcademy-FullStack-T14/blob/lectures/lecture-03-css-scss/course-materials/l03_css_scss/css%20-%20specificity.pdf)

优先级高的设置会覆盖上一级的设置，selector 越详细，优先级越高。

## [00:36:30] BEM - Block Element Modifier

Block

```css
.stick-man {
}
```

Element

Modifier

<br>
<hr>
<hr>

## _[Switch to [Responsive Web Design](03_responsiveDesign.md)]_

## [00:10:00] CSS Properties

### Padding

### Box Width

### Display and Visibility

### Position

### Float and Clear
