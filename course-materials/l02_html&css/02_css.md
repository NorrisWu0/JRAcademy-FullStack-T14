[回到目录](../../README.md)

<hr>
<hr>
<br>

# | CSS - Cascading Style Sheets |

本部分内容包括，`css`的介绍及背景，编写`css`的方式，如何通过 Dev Tools 来查看`css`效果，selector，unit，box model。

<hr>

## [Part 2 - 01:44:50] What is CSS

CSS 是一种用于表达及定义网页内容样式的语言，CSS 能决定网页元素会如何呈现在屏幕上，纸质或其他种类的媒介上。

- CSS1：发行于 1996 年，当时的`css`只包含 Fonts, Colors, Alignment, Spacing.
- CSS2.1：2004 年，添加了对 Layout, positioning 的支持。
- CSS3：最新版，添加了对 Effects, sizing, speech 及其他功能的支持。
  <br>

---

## [Part 2 - 01:46:00] How does CSS work?

浏览器会将`html`和`css`转换成`DOM (Document Object model)`。`DOM`则会集合页面的内容及相对应的 style，存储在电脑的内存中。浏览器再从内存中读取`Dom`并将其显示在屏幕上。

![How Css Work](/l02_html&css/note-assets/how-css-work.png)

**推荐阅读:**
[W3Schools CSS Tutorial](https://www.w3schools.com/css/) |
[How dose CSS actually work?](https://www.youtube.com/watch?v=tSv2KIF7uE4)

<br>

---

## **[Part 2 - 01:49:20] Types of Style Sheet**

`css`有三种编写方式，External，Internal 或 Inline。

### **外部导入（External）- 推荐：**

External `css` 一般会存在以`.css`结尾的文件内，`html`文件则会通过导入`style.css`文件（External）来给元素定义样式。他们通常看起来像这样。

> 输入:
>
> ```css
> /* style.css */
>
> div {
>   padding: 1em;
>   background-color: #101010;
>   color: white;
>   text-align: center;
> }
>
> p {
>   font-family: verdana;
>   font-size: 20px;
> }
> ```
>
> ```html
> <!-- index.html -->
>
> <!DOCTYPE html>
> <html>
>   <head>
>     <link rel="stylesheet" href="styles.css" />
>   </head>
>   <body>
>     <div>
>       <h1>Hello World!</h1>
>       <p>I'm a html page with external styling.</p>
>     </div>
>   </body>
> </html>
> ```
>
> 输出:
>
> <div style="padding: 1em; background: #101010; color: white; text-align: center">
>   <h1>Hello world</h1>
>   <p style="font-family: verdana; font-size: 20px;">I'm a html page with external styling.</p>
> </div>

这种方法的优势在于它可以被导入在不同的 html 文件中以及能更方便地被管理。

<br>

### **内部编写（Internal）- 不推荐：**

Internal 则是在`html`中添加`<style></style>`标签并编写。

> 输入：
>
> ```html
> <!-- index.html -->
>
> <!DOCTYPE html>
> <html>
>   <head>
>     <style>
>       div {
>         padding: 1em;
>         background: #101010;
>         color: white;
>         text-align: center;
>       }
>       p {
>         font-family: verdana;
>         font-size: 20px;
>       }
>     </style>
>   </head>
>   <body>
>     <div>
>       <h1>Hello World!</h1>
>       <p>I'm a html page with internal styling.</p>
>     </div>
>   </body>
> </html>
> ```
>
> 输出:
>
> <div style="padding: 1em; background: #101010; color: white; text-align: center">
>   <h1>Hello world</h1>
>   <p style="font-family: verdana; font-size: 20px;">I'm a html page with internal styling.</p>
> </div>

这种方式虽然能达到同样的效果，但是存在的问题是他不能跟其他的`html`文件共享样式，并且这类样式会更难管理及维护。

<br>

### **同行编写（Inline）- 不推荐：**

Inline `css` 一般则会直接出现在`html`元素的标签上，他们通常看起来像这样。

> 输入：
>
> ```html
> <!-- index.html -->
>
> <!DOCTYPE html>
> <html>
>   <head></head>
>   <body>
>     <div
>       style="padding: 1em; background: #101010; color: white; text-align: center"
>     >
>       <h1>Hello world</h1>
>       <p style="font-family: verdana; font-size: 20px;">
>         I'm a html page with inline styling.
>       </p>
>     </div>
>   </body>
> </html>
> ```
>
> 输出：
>
> <div style="padding: 1em; background: #101010; color: white; text-align: center">
>   <h1>Hello world</h1>
>   <p style="font-family: verdana; font-size: 20px;">I'm a html page with inline styling.</p>
> </div>
> 这种方式存在和Internal `css`一样的问题。

<br>

---

## **[Part 2 - 01:56:30] Dev Tool**

浏览器自带的开发者工具能帮助你细致的审查你的`css`。在 Chrome 浏览器中，有两种方式可以打开开发者工具。

- 通过点击右上角的菜单键（图标为竖向排列的三个点），选择 More tools，然后 Developer tools 来打开开发者工具。
- 在页面任意处右键，点击 Inspect Element 会打开开发者工具，并跳转到你所点击的元素上。
- 在 Windows 平台上可以通过按 `Ctrl+Shift+I`或`F12`快捷键打开开发者工具。

![Chrome Dev Tools](/l02_html&css/note-assets/chrome-dev-tools.png)

通常开发者工具都会分类不同的功能标签，例如 Element, Console, Source 等。

### Element -

### 开发小提示:

你可以通过按`Windows Key + R`后输入`cmd`打开命令台，并在命令台里输入`npm install live-server -g`来安装`html`实时服务器插件。然后通过运行插件后在浏览器上实时查看你的网页输出后的样子。

<br>

---

## **[Part 2 - 01:58:30] Style Rules**

---

use class most of time
ID is exclusive per element

lots of selector stuffs

<br>

## **[Part 2 - 02:14:51] Box Model**

---

<br>

## **[Part 2 - 02:33:25] Units**

---

<br>

## **[Part 2 - 02:50:00] Button**

---

[Block Element Modifer](http://getbem.com/introduction/)

Block
.card

Element
.card-title
.card-desc
.card-button

Modifier
.card-button-disabled

<br>

## **[::] **

---
