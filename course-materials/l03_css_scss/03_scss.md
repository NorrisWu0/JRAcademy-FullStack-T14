[回到目录](../../README.md)

<hr>
<hr>
<br>

# | Sass - CSS Preprocessor |

## [:] **CSS Preprocessor**

### **Preprocessor 种类**

- [Less](https://lesscss.org/)
- [Sass](https://sass-lang.com/)
- [PostCSS](https://postcss.org/)

<br>

---

## [:] **Sass**

[Sass 文档](https://sass-lang.com/documentation)

### **安装方式**

`npm install sass -g`

<br>

### [:] **优势**

- 简化编写过程，加快开发速度。
- 更容易管理及维护代码。

<br>

### [:] **例子**

> 编写`style.scss`文件：
>
> ```css
> /* style.scss */
> nav {
>   ul {
>     margin: 0;
>     padding: 0;
>     list-style: none;
>   }
>   li {
>     display: inline-block;
>   }
>   a {
>     display: block;
>     padding: 6px 12px;
>     text-decoration: none;
>   }
> }
> ```
>
> Sass 文件 compile 后生成`style.css`：
>
> ```css
> /* style.css */
> nav ul {
>   margin: 0;
>   padding: 0;
>   list-style: none;
> }
>
> nav li {
>   display: inline-block;
> }
>
> nav a {
>   display: block;
>   padding: 6px 12px;
>   text-decoration: none;
> }
> ```

<br>

### [:] **Sass 常用命令**

- `nested`: 嵌套缩进的`css`代码，为默认值。
- `expanded`: 没有缩进的，拓展的`css`代码。
- `compact`: 简介格式的`css`代码。
- `compressed`: 压缩后的`css`代码。

<br>

### [:] **使用方式**

当编写完`style.scss`后，有不同的方式来生成所需的`style.css`文件。

#### [:] 手动转换

在 terminal 中运行`sass --style compressed ./style.scss ./style.min.css`。将所编写的`style.scss`compile 成浏览器能识别的`style.min.css`。其中"`min`"代表缩减后的格式。

> `style.min.css`例子
>
> ```css
> /* nav ul {margin:0;padding: 0;list-style: none;} nav li {display: inline-block;} nav a {display: block;padding: 6px 12px;text-decoration: none;} */
> ```

#### [:] 设立监听

在 terminal 中运行下面的代码来生成`css`文件。

- 监听指定文件: `sass --watch input.scss:output.css`
- 监听指定文件夹: `sass --watch app/sass:public/stylesheet/`

#### [:] 使用插件（个人推荐）

> Name: Live Sass Compiler
>
> Id: ritwickdey.live-sass
>
> Description: Compile Sass or Scss to CSS at realtime with live browser reload.
>
> Version: 3.0.0
>
> Publisher: Ritwick Dey
>
> VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass

启动后在保存 Sass 文件是会自动 compile.

<br>

### [:] **@import**

Sass 还能其文件中导入其他的自己编写的 Sass 文件，方便开发管理代码库。例如在 `style.scss`中可以导入`colors.scss`来使用被导入的 Sass 文件参数。

> ```css
> /* colors.scss */
> $primaryColor: #eeffcc;
> $accentColor: #ddeebb;
>
> /* style.scss */
> @import 'colors';
>
> body {
>   background: $primaryColor;
>   color: $accentColor;
> }
> ```

<br>

### [:] **Sass 变量（Variable）**

Sass 文件也有相应的变量功能，变量为所开发的网页提供了统一性。开发可以通过使用变量管理多个元素的样式或管理页面的可兼容性。

> ```css
> /* Color Variable */
> $primaryColor: #eeffcc;
> $accentColor: #ddeebb;
>
> /* Media Queries Variable*/
>
> $screenSmMin: 768px !default;
> $screenMdMin: 992px !default;
> $screenLgMin: 1200px !default;
>
> /* Breakpoints */
> $small: new-breakpoint(max-width $screenSmMin);
> $medium: new-breakpoint(max-width $screenMdMin);
> $mobileSm: new-breakpoint(max-width $mobilemSm);
> $tiny: new-breakpoint(max-width $tinyMobileMax);
> $mobile: new-breakpoint(max-width $mobileMax);
> ```

<br>

### [:] **Sass 数学**

Sass 文件也支持数学公式的运算。

> ```css
> $container-width: 100%;
> .container {
>   width: $container-width;
> }
> .col-4 {
>   width: $container-width / 4;
> }
> ```

<br>

### [:] **Sass Nesting**

> ```css
> /* style.scss */
> a.myAnchor {
>   color: blue;
>   &:hover {
>     text-decoration: underline;
>   }
>   &:visited {
>     color: purple;
>   }
> }
>
> /* style.css */
> a.myAnchor {
>   color: blue;
> }
> a.myAnchor:hover {
>   text-decoration: underline;
> }
> a.myAnchor:visited {
>   color: purple;
> }
> ```

<br>

### [:] **Sass 继承**

> ```css
> /* style.scss */
> .class1 {
>   border: 1px solid #ddd;
> }
> .class2 {
>   @extend .class1;
>   font-size: 120%;
> }
>
> /* style.css */
> .class1 {
>   border: 1px solid #ddd;
> }
> .class2 {
>   border: 1px solid #ddd;
>   font-size: 120;
> }
> ```

<br>

### [:] **Sass Mixins**

使用`@mixin`定义一个代码块，并使用`@include`来调用这个 mixin

> ```css
> @mixin media(&queryString) {
>   /* some code */
> }
>
> div {
>   @include media;
> }
> ```
