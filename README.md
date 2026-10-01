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

## 3. **Use inline**
Tailwind CSS's inline utility makes an element an inline-level element.
```
<div>
  <span class="inline bg-blue-500">
    Hello
  </span>
  <span class="inline bg-red-500">
    World
  </span>
</div>
```
**Here:**
*`inline* → keeps the element on **the same line**.<br>
It normally takes only the **width required by its content**.<br>
The next inline element can **appear on the same line**.<br>
**Simple rule:**<br>
*`inline` → makes an element **inline-level and helps keep elements** on the same line.
## 4. **Use inline-block**
Tailwind CSS's `inline-block` utility makes an element an **inline-block element**.
```
<span class="inline-block bg-blue-500 p-4">
  Hello
</span>
<span class="inline-block bg-red-500 p-4">
  World
</span>
```
**Here**:<br>
inline-block → elements can stay on **the same line**.<br>
*`p-4` → **applies padding**.<br>
*`bg-blue-500` → gives the element a **background color**.<br>
The advantage of `inline-block` is that the element stays on the **same line like inline**, but you can properly **control its width, height, padding, and margin**.<br>
Simple rule:<br>
*`inline` → same line **+ limited box control**<br>
*`inline-block` → same line **+ width/height/padding/margin** control
## 5. **Use flex**
Tailwind CSS's flex utility makes an element a **flex container**. It allows you to **easily arrange and align its child elements**.
```
<div class="flex">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
By default, the items appear in a **row (horizontal) direction**.
Example with gap
```
<div class="flex gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
</div>
```
**Here:**<br>
*`flex` → enables the **Flexbox layout**.<br>
*`gap-4` → **adds space** between the items.<br>
*`p-4` → **adds padding inside** each item.<br>
**Simple rule:**<br>
*`flex` → used to arrange child elements in a flexible layout.
## 6. **Use flex-row**
Tailwind CSS's **flex-row utility arranges flex items in a horizontal direction**.
```
<div class="flex flex-row">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
**Output:**
```
One   Two   Three
```
**Here:**<br>
*`flex` → **enables the Flexbox layout**.<br>
flex-row → arranges items from **left to right (horizontal)**.<br>
**Simple rule**:<br>
*`flex-row` → Flex items are **arranged in a row (horizontal)**.
## 7. **Use flex-col**
Tailwind CSS's **flex-col utility** arranges flex items in a **vertical direction**.
```
<div class="flex flex-col">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
**Output:**
```
One
Two
Three
```
**Here:**<br>
*`flex` → enables **the Flexbox layout**.<br>
*`flex-col` → arranges items from **top to bottom (vertical)**.<br>
**Simple rule:**<br>
*`flex-col` → Flex items are **arranged in a column (vertical)**.
## 8. **Use flex-wrap**
Tailwind CSS's flex-wrap utility is used to move flex items to the next line (wrap) when there is not enough space in the container.
```
<div class="flex flex-wrap gap-4">
  <p class="w-40 bg-blue-500 p-4">One</p>
  <p class="w-40 bg-red-500 p-4">Two</p>
  <p class="w-40 bg-green-500 p-4">Three</p>
  <p class="w-40 bg-yellow-500 p-4">Four</p>
</div>
```
**Here:**<br>
*`flex` → **enables Flexbox**.<br>
*`flex-wrap` → allows items to **wrap to the next line**.<br>
*`gap-4` → **adds space between** the items.<br>
*`w-40` → **sets the width** of each item.<br>
Simple rule:<br>
flex-wrap → When there isn't enough space in one row, items move to the next line.
