[回到目录](../../README.md)

<hr>
<hr>
<br>

# | HTML - HyperText Markup Language |

### **[Part 1 - 20:00] What is HTML?**

[What Really Happens When you visited a website?](youtube.com/watch?v=z0HN-fG6oT4)
Browser

HTML is not programming language, it's markup language!

<br>

### **[Part 1 - 30:00] How HTML, CSS & JavaScript work together**

[HTML, CSS & Javascript Explained](https://www.youtube.com/watch?v=gT0Lh1eYk78)

**HTML** construct the framework of an webpage, **Cascading Style Sheets - CSS** Beautify the framework HTML constructed, **JavaScript** handles the user input to provide interactivity.

Q: What about React?
React is a framework, it's not part of the first 3 lectures.

Javascript Fatigue.

<br>

### **[Part 1 - 36:50] Your Best Friend**

---

Web Development Dictionary

1. [W3School]
2. [Mozella Developer Network]

<br>

### **[Part 1 - 38:40] HTML + CSS + JS**

---

<br>

### **[Part 1 - 39:00] HTML**

---

can use `!` or `html` to create a html template.

Meta datas - default with ^ creation

- `<meta charset="UTF-8" />` - must have to decode multiple language.
- `<meta http-equiv="X-UA-Compatible" content="IE=edge">` - support for older browser
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">` - responsive setting>

<br>

- `<title>Document</title>` 网页标题
- ``
- [Material Design Icon](https://fonts.google.com/icons?selected=Material+Icons)

<br>

**[Part 1 - 58:50 - 1:00:00]semantic & SEO**

<br>

Live server - `npm install -g live-server`
可让浏览器实时更新所读取文件

<br>

_Lecture disconnected at [01:00:00]_
_Lecture on break for 10 mins, recommence at [07:38pm]_

<br>

### **[Part 2 - 17:12] Chrome Dev Tool**

---

- Performance - 加载时间 读取时间
- Memory - 内存使用状况
- Application - 类似文件浏览器，可查看本地存储，
- Security - 查看网页是否安全，数据是否加密
- Lighthouse - 查看网页性能，可生成页面性能报告
- Axe Dev Tools - 查看页面 Accessibility

<br>

### **[Part 2 - 26:30] Personal Website**

---

[Portfolio Sample 1](https://australiaitgroup.github.io/jrprofile/#home) | [Sample Source Code](https://github.com/australiaitgroup/jrprofile)

\*[28:30]SEO - Search Engine Optimization
搜索引擎会读取`<head> tag`中的 meta data 来判断页面的内容。

Example from [匠人课堂](https://learn.jiangren.com.au/home):

```html
<meta
  name="description"
  content="澳洲最大的学习就业平台, 免费学习大学课程, 大学内容辅导, 制作简历, 招聘信息等"
/>
<meta
  name="keywords"
  content="澳洲学习,大学学习,简历制作,简历定制,工作内推,实习求职,学习平台,大学辅导,大学生找工作,大学补习"
/>
```

<br>

### **[Part 2 - 33:00] Structure**

---

<br>

### **[Part 2 - 33:00] HTML Basics + Head + Body**

---

<br>

### **[Part 2 - 33:50] Block vs Inline**

---

- Block Element - 占据整行空间，有 padding 且有 margin。

  包括 `<div> <header> <main> <nav> <section> <footer`

- Inline Element - 只占据内容空间，无 padding 且无 margin。

  _\*注意语义性(semantic), 可以查看 [W3C](https://www.w3schools.com/html/html_blocks.asp), [MDN Block Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements) 和 [MDN Inline Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements)来查看用法._

<br>

### **[:] Text - Header**

---

<br>

### **[Part 2 - 43:50] SEO**

---

Only one H1 for one page

- Page Structure
- H1
- H2
- H2
- H3
- H3
- H4
- H4
- H4
- H5
- H5
- H5
- H6
- H6
- H6

<br>

### **[:] Text - Header**

---

<br>

### **[Part 2 - 45:05] Paragraph**

---

`<p>`是 paragraph element。

<br>

### **[Part 2 - 46:30] Text - Format Element**

---

`<strong>`对于浏览器来说有语义，所以还在使用

尽量使用 css 来 styling，而不是依赖 html tag 来 styling

<br>

### **[Part 2 - 50:00] Span**

---

`<span>`用于 style 行内单独 element。

<br>

### **[Part 2 - 52:00] [List](https://www.w3schools.com/html/html_lists.asp)**

---

通用于 navigation bar 中，

```html
<ul>
  // unordered list
  <li>list item</li>
  // - item 1
  <li>list item</li>
  // - item 2
  <li>list item</li>
  // - item 3
</ul>

<ol>
  // ordered list
  <li>list item</li>
  // 1. item 1
  <li>list item</li>
  // 2. item 2
  <li>list item</li>
  // 3. item 3
</ol>
```

<br>

### **[Part 2 - 53:20] [Table](https://www.w3schools.com/html/html_tables.asp)**

---

```html
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```

<br>

### **[Part 2 - 56:30] [div element](https://www.w3schools.com/tags/tag_div.ASP)**

---

<br>

### **[Part 2 - 57:00] [link element](https://www.w3schools.com/html/html_links.asp)**

---

[iFrame Element](https://www.w3schools.com/html/html_iframe.asp)

<br>

### **[Part 2 - 01:00:00] [Img Element](https://www.w3schools.com/html/html_images.asp)**

---

- `<img src="pic_trulli.jpg" alt="Italian Trulli">`
  src 会读取图片文件，alt 会在图片加载不出来时用文字替代图片内容。

- `src="./img.png"`会读取当前目录下的文件。
- `src="../img.png"`会读取上级目录的文件。
- `src="/img/img.png`会从根目录开始追踪文件文件位置，具有不需要考虑相对路径的优势。

<br>

### **[Part 2 - 01:00:] [File Path]()**

---

<br>

### **[Part 2 - 01:22:00] [Form & Input](https://www.w3schools.com/html/html_forms.asp)**

---

> 输入:
>
> ```html
> <form>
>   <label for="fname">First name:</label>
>   <br />
>   <input type="text" id="fname" name="fname" />
>   <br />
>   <label for="lname">Last name:</label>
>   <br />
>   <input type="text" id="lname" name="lname" />
> </form>
> ```
>
> 输出:
>
> <form>
>  <label for="fname">First name:</label><br>
>  <input type="text" id="fname" name="fname"><br>
>  <label for="lname">Last name:</label><br>
>  <input type="text" id="lname" name="lname">
> </form>
> <br>

`action="some action"`不再用了，`value="some value"`也不用了。

<br>

### **[Part 2 - 10:28:20] HTML5 Input**

---

<br>

### **[Part 2 - 10:32:00] HTML5 Semantic**

---

可以查看来看[HTML tags](https://www.tutorialrepublic.com/html-reference/html5-tags.php)如何使用 tag 来提高语义性。

<br>

### **[Part 2 - 01:35:25] Comment**

---

最好的代码是 self documenting code。
备注解释的不是代码的作用，而是逻辑及代码目的。

<br>

### **[Part 2 - 01:38:50] Can I Just Use html5 Elements?**

---

可以用[Can I use.com](https://caniuse.com/)判断 element 能在哪些平台上正常运作，检查代码的平台适应性。

<br>

### **[Part 2 - 01:42:10] HTML Best Practices**

---

<br>

### **[Part 2 - 01:42:20] HTML Interview Questions**

---

[HackerRank](https://www.hackerrank.com/)

<br>

_[01:43:20] End of HTML topic_
