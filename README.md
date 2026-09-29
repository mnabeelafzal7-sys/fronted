# **Layout Mastery**
## 1. **Understand CSS box model through Tailwind**
The CSS **Box Model** means that every **HTML element** is considered a box.**This box has 4 main parts:**<br>
### **Content → Padding → Border → Margin**<br>
In Tailwind CSS, we control these using **utility classes.**
```
<div class="w-64 p-4 border-2 m-4">
  Content
</div>
```
* `w-64` → **Content/element width**
* `p-4` → **Padding** — content aur border ke darmiyan space
* `border-2` → **Border** — element ke around line
* `m-4` → **Margin** — element ke bahar space<br>
**In tailwind**
`w/h` → size
`p-*` → padding
`border-*` → border
`m-*` → margin
## 2. **Use block**
Tailwind CSS mein `block` utility element ko **block-level element** banati hai.
```
<div class="block">
  Hello World
</div>
```
Use this class in side **element blocks**.
```
<span class="block bg-blue-500 p-4">
  Hello World
</span>
```
**Yahan:**
* `block` → element ko new line par rakhta hai
* `bg-blue-500` → background color
* `p-4` → padding
Simple: block → element ko block-level banata hai.
